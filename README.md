# Bridge2AI 🚧🚧
This API is a solution for developers who want to use [OpenAI's](https://platform.openai.com/overview) text and image generation technology in their applications. With multiple endpoints available, it is possible to generate text, images, and edit images using specific prompts and models.

## How to use
To use this API, it is necessary to send an HTTP request to one of the available endpoints, providing the necessary inputs for text or image generation. It is important to note that the API performs validations to ensure that the inputs are valid before sending requests to OpenAI to ensure accurate and relevant responses.

Please include that to use the API, the user needs to add the API key generated on the OpenAI website, and the billing is based on usage, but it is very affordable compared to the rate set by the "plus" of [ChatGPT](https://chat.openai.com/chat).

## Endpoints

#### `completion`
This endpoint allows for text generation based on input text and a prompt. It is necessary to provide input text and a prompt as inputs in the HTTP request. The endpoint will return a response generated by OpenAI based on that input.

#### `image`
This endpoint allows for image generation based on a prompt, image model, and image size. It is necessary to provide a prompt, image model, and image size as inputs in the HTTP request. The endpoint will return an image generated by OpenAI based on those inputs.

#### `image-edit`
This endpoint allows for image editing based on input images, a mask, and a prompt. It is necessary to provide input images, a mask, and a prompt as inputs in the HTTP request. The endpoint will return an image edited by OpenAI based on those inputs.


# Bridge2AI

This API is a solution for developers who want to use OpenAI's text and image generation technology in their applications. With multiple endpoints available, it is possible to generate text, images, and edit images using specific prompts and models.

Clone the project

```bash
  git clone https://github.com/matheuskroska/Bridge2AI.git
```

Go to the project directory

```bash
  cd my-project
```

Install dependencies

```bash
  npm install || yarn
```

Start

```bash
  node index
```



## API Documentation

#### Returns a text generated by the OpenAI API based on the provided prompt.

```http
  POST /completion
```

### Request Body

| Parameter   | Type       | Description                                   |
| :---------- | :--------- | :------------------------------------------ |
| `prompt`      | `string` | 	A string representing the prompt to generate text completion for.|


### Query Parameters

| Parameter   | Type       | Description                                   |
| :---------- | :--------- | :------------------------------------------ |
| `max_tokens`      | `integer` | 	The maximum number of tokens to generate. Defaults to 50.|
| `temperature`      | `float` |A number from 0 to 1 that determines the 'creativity level' of the generated text. The closer to 0, the more conservative the text will be. The closer to 1, the more creative and unpredictable the text will be. Default: 0.|








### Conclusion
Bridge2AI is a powerful and secure tool for interacting with OpenAI's generation API. With text, image, and image editing endpoints available, it is possible to explore the possibilities offered by OpenAI and create innovative and impressive applications.

