FROM python:3.11
RUN pip install llm
RUN UNAME_M=arm64 UNAME_p=arm LLAMA_NO_METAL=1 llm install llm-llama-cpp llama-cpp-python==0.1.77
RUN llm llama-cpp download-model https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/resolve/main/llama-2-7b-chat.ggmlv3.q8_0.bin --alias l2c
ENTRYPOINT ["llm", "-m", "l2c"]