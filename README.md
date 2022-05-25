# BERT
영어 한국어 버트

# 1. 
pip install transformers


# 2.
import tensorflow as tf

from transformers import TFBertForNextSentencePrediction

from transformers import AutoTokenizer

# 3.

model = TFBertForMaskedLM.from_pretrained('klue/bert-base', from_pt=True)

tokenizer = AutoTokenizer.from_pretrained("klue/bert-base")


# 4.

from transformers import FillMaskPipeline

pip = FillMaskPipeline(model=model, tokenizer=tokenizer)

# 5.
pip('축구는 정말 재미있는 [MASK]다.')

참고 문헌 : https://wikidocs.net/22592
