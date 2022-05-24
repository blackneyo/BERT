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

pip('어벤져스는 정말 재미있는 [MASK]다.')

pip('나는 오늘 아침에 [MASK]에 출근을 했다.')
