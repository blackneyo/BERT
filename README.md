# BERT
영어 한국어 버트

# 1. 필요 라이브러리 설치
pip install transformers

import tensorflow as tf

from transformers import TFBertForNextSentencePrediction

from transformers import AutoTokenizer

# 2. 학습된 모델 불러오기

model = TFBertForMaskedLM.from_pretrained('klue/bert-base', from_pt=True)

tokenizer = AutoTokenizer.from_pretrained("klue/bert-base")


# 4.

from transformers import FillMaskPipeline

pip = FillMaskPipeline(model=model, tokenizer=tokenizer)

# 5.
pip('축구는 정말 재미있는 [MASK]다.')

참고 문헌 : https://wikidocs.net/22592
