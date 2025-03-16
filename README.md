# Aya-Vision LitServe

[![Open In Studio](https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/app-2/studio-badge.svg)](https://lightning.ai/sitammeur/studios/deploy-paligemma-2-mix-vision-language-model)

C4AI [Aya Vision](https://huggingface.co/collections/CohereForAI/c4ai-aya-vision-67c4ccd395ca064308ee1484) is an open weights research release featuring models that offers advanced capabilities optimized for a variety of vision-language applications, including optical character recognition (OCR), captioning, visual reasoning, summarization, question answering, and coding, among others. This multilingual model has been trained to excel in 23 languages across both vision and language tasks. This project shows how to create a self-hosted, private API that deploys [Aya Vision 8B](https://huggingface.co/CohereForAI/aya-vision-8b) model variant with LitServe, an easy-to-use, flexible serving engine for AI models built on FastAPI.

## Project Structure

The project is structured as follows:

- `server.py`: The file containing the main code for the web server.
- `client.py`: The file containing the code for client-side requests.
- `LICENSE`: The license file for the project.
- `README.md`: The README file that contains information about the project.
- `assets`: The folder containing screenshots for working on the application.
- `images`: The folder containing images for testing purposes.
- `.env.example`: The example file for environment variables.
- `.gitignore`: The file containing the list of files and directories to be ignored by Git.

## Tech Stack

- Python (for the programming language)
- PyTorch (for the deep learning framework)
- Hugging Face Transformers Library (for the model)
- LitServe (for the serving engine)

## Getting Started

To get started with this project, follow the steps below:

1. Run the server: `python server.py`
2. Upon running the server successfully, you will see uvicorn running on port 8000.
3. Open a new terminal window.
4. Run the client: `python client.py --image <image_path> --prompt "<prompt>"`.

Now, you can see the model's output based on the input request. The model will provide responses for the images in the `images` folder based on the questions you ask in all 23 languages the model supports.

**Note**: You need a Hugging Face access token to run the application. You can get the token by signing up on the Hugging Face website and creating a new token from the settings page. After getting the token, you can set it as an environment variable `ACCESS_TOKEN` in your system by creating a `.env` file in the project's root directory. Check the `.env.example` file for reference.

## Usage

The project can be used to serve the Aya Vision family of models using LitServe. It allows you to input an image and a prompt (can be multilingual) and get the model's output based on the input. The model can be used for various vision-language tasks such as optical character recognition (OCR), captioning, visual reasoning, summarization, question answering, coding, and others.

## Contributing

Contributions are welcome! If you would like to contribute to this project, please raise an issue to discuss the changes you want to make. Once the changes are approved, you can create a pull request.

## License

This project is licensed under the [Apache-2.0 License](LICENSE).

## Contact

If you have any questions or suggestions about the project, feel free to contact me on my GitHub profile.

Happy coding! 🚀
