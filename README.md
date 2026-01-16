# This repo is abandoned
I no longer add new models to this repo, because of the lack of public interest. Repo is still open for PRs.

### AI Model-Mappings
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

### Wavespeed
The [documented](https://wavespeed.ai/docs/docs-common-api/models#example-request) endpoint returns 404, use this fixed request:
```
curl https://api.wavespeed.ai/api/v3/models
  -H "Authorization: Bearer YOUR_API_KEY" > wavespeed_official.json
```
or unofficial alternative:
```
curl 'https://wavespeed.ai/center/default/api/v1/model_product/find' \
  --data-raw '{"page":1,"page_size":999}' > wavespeed_unofficial.json
```

### NanoGPT
```
curl --request GET \
  --url https://nano-gpt.com/api/models > nanogpt_models.json
```

### Chutes
```
curl -X GET "https://api.chutes.ai/chutes/?template=diffusion" \
  -H "Content-Type: application/json" > chutes_models.json
```
