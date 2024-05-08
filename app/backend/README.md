# Backend

The backend is located in the `app/backend` directory.

## Main Libraries and Services

- **Azure services**: The backend uses various Azure services like Azure Search, Azure Blob Storage, and Azure Key Vault. These are handled by their respective clients such as [`SearchClient`](https://docs.microsoft.com/python/api/overview/azure/search-documents-readme?view=azure-python), [`ContainerClient`](https://docs.microsoft.com/python/api/overview/azure/storage-blob-readme?view=azure-python), and [`SecretClient`](https://docs.microsoft.com/python/api/overview/azure/keyvault-secrets-readme?view=azure-python).
- **OpenAI**: The `AsyncOpenAI` class is used for interactions with the OpenAI API.
- **Quart**: The [`Quart`](https://pgjones.gitlab.io/quart/) library is used to create the web application.

## Running the Backend Locally

To run the backend locally, you can use the "Start App" task defined in the tasks.json file. This task runs the `start.sh` or `start.ps1` script depending on your operating system.

For more details on local development, refer to the local development guide.

## Deployment

The backend is deployed as part of the overall application. For details on deployment, refer to the README.

# Python Dependencies

This document lists the Python packages that are required for this project.

## Package Descriptions

- **types-html5lib (1.1.11.20240228)**: Type stubs for html5lib, required by types-beautifulsoup4.
- **types-pillow (10.2.0.20240213)**: Type stubs for Pillow, a Python Imaging Library.
- **types-pyasn1 (0.6.0.20240402)**: Type stubs for pyasn1, required by types-python-jose.
- **types-python-jose (3.3.4.20240106)**: Type stubs for python-jose, a JOSE implementation in Python.
- **types-pytz (2024.1.0.20240203)**: Type stubs for pytz, required by pandas-stubs.
- **typing-extensions (4.10.0)**: Backported and experimental type hints, required by multiple packages including azure-ai-documentintelligence, azure-core, azure-keyvault-secrets, azure-storage-blob, azure-storage-file-datalake, openai, opentelemetry-sdk, pydantic, and pydantic-core.
- **tzdata (2024.1)**: Timezone database in Python, required by pandas and pendulum.
- **urllib3 (2.2.1)**: HTTP library with thread-safe connection pooling and file post support, required by requests.
- **uvicorn (0.27.1)**: The lightning-fast ASGI server.
- **werkzeug (3.0.1)**: A comprehensive WSGI web application library, required by flask and quart.
- **wrapt (1.16.0)**: A module for decorators, wrappers and monkey patching, required by deprecated and opentelemetry-instrumentation.

## Installation

To install these packages, run the following command:

```bash
pip install -r requirements.txt