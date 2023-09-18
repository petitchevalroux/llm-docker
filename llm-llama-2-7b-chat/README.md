## Build
```
docker build . -t petitchevalroux/llm-llama-2-7b-chat
```

## Push to dockerhub
```
docker push petitchevalroux/llm-llama-2-7b-chat
```

## Usage
### Using command line argument
```
docker run petitchevalroux/llm-llama-2-7b-chat "what is the capital of France?"
```
Output :
```
The capital of France is Paris.
```
### Using unix pipe
```
echo "what is the capital of france ?" | docker run -i petitchevalroux/llm-llama-2-7b-chat
```
Output :
```
- The capital of France is Paris.
```
