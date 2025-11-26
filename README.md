# AI Model-Mappings
Providers are a bit too creative with model names, serving the same model but under a different name. This repo maps them together.

# Contributing
While I'm focused on Image and Video models, other models are welcome to be added. Please add them to the `map.js` file and open a pull request.




## Download Model lists

### Fal
```bash

curl --request GET \
  --url https://api.fal.ai/v1/models?limit=1000 \
  --header 'Authorization: Key <YOUR_API_KEY>:<YOUR_API_SECRET>' > fal-models.json
```
