# computer-vission-azure
Analyze Images with Azure AI Computer Vision
Azure AI Vision provides artificial intelligence capabilities to analyze visual input by analyzing images. The service includes models for common computer vision tasks, such as generating captions, identifying common objects, detecting landmarks, and moderating content.

Clone the Repository for This Course
Open Visual Studio Code.
Use the Git: Clone command to clone the AI-102-AIEngineer repository.
Open the cloned folder in Visual Studio Code.
Provision an Azure AI Services Resource
Open the Azure portal at https://portal.azure.com.

Search for "Azure AI Services" and create an Azure AI multi-service account with the following settings:

Subscription: Your Azure subscription.
Resource group: Choose or create a resource group.
Region: Select an available region.
Name: Enter a unique name.
Pricing tier: Standard S0.
After deployment, access the Keys and Endpoint page to retrieve necessary credentials.

Prepare to Use the Azure AI Vision SDK
In Visual Studio Code, navigate to the appropriate language folder (C# or Python).

Open an integrated terminal in the image-analysis folder.

Install the Azure AI Vision SDK:

C#:

dotnet add package Microsoft.Azure.CognitiveServices.Vision.ComputerVision --version 6.0.0
Python:

pip install azure-cognitiveservices-vision-computervision==0.7.0
Create a .env file in the root directory.

Add your Azure Vision API credentials:

AI_SERVICE_ENDPOINT=your_azure_endpoint
AI_SERVICE_KEY=your_azure_key
Replace your_azure_endpoint and your_azure_key with your actual Azure
##Output

-Original Image street

-Modified(Analyzed) Screenshot Screenshot 2024-10-28 105001
![Uploading image.png…]()


Analyze Images
Authenticate the Azure AI Vision client using your credentials.
Specify features to retrieve, such as captions, tags, and categories.
Implement image analysis functions in the code file.
Run the program with sample images and observe the output captions, tags, and detected objects.
Additional Features
Thumbnail Generation: Crop and create a smaller version of the image focusing on the main subject.
Moderation Ratings: Detect and classify images as adult, racy, or gory based on content.
Brands and Objects Detection: Identify brands and specific objects with bounding boxes.
