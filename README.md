# AI Transcription & Content Generation (All-in-One)
This Google Colab notebook provides an automated workflow to transcribe audio/video files and generate AI-powered content based on the transcriptions.

**✨ Features**
Multilingual Transcription: Automatically transcribes audio/video files using OpenAI's Whisper model, supporting various languages.
Google Drive Integration: Connects to your Google Drive to find new media files and save processed outputs.
Intelligent Content Generation: Leverages Google's Gemini AI to create:
Meeting Notes: Structured summaries from meeting transcripts.
Content Ideas: Suggestions for LinkedIn posts or other content based on discussions.
Meeting Analysis: Provides insights into meeting effectiveness (e.g., 'Could This Have Been an Email?' score, 'Meeting Quality Score').
Automated File Management: Organizes your files by moving processed audio to a dedicated folder and storing transcripts and AI-generated content in structured subdirectories.

**📝 How to Use**
Open in Google Colab: Open this notebook in Google Colab.
Configure Parameters: In the first code cell, adjust the following parameters:
main_project_folder: The name of your main project folder in Google Drive where your audio/video files are located.
audio_language: Select the language of your audio files for accurate transcription.
transcription_model_size: Choose a Whisper model size (e.g., 'medium' for a good balance).
Check the boxes for generate_meeting_notes, generate_content_ideas, and generate_meeting_analysis if you want these AI features enabled.
Run the Cell: Click the 'Play' button (▶️) on the first code cell to start the entire process.
Authorize Google Drive: Follow the prompts to authorize Google Drive access.
Provide Gemini API Key: Ensure your GEMINI_API_KEY is set in Google Colab secrets. If not, the AI content generation steps will be skipped.

**📂 Output Structure**
Within your main_project_folder (or the folder where your audio files reside), the notebook will create the following subfolders:
01_Completed_Transcripts: Contains .txt files of the transcribed audio.
02_AI_Generated_Content: Contains subfolders for:
Meeting_Notes: Markdown files with meeting summaries.
Content_Ideas: Markdown files with content ideas.
Meeting_Analysis: Markdown files with meeting analysis.
03_Processed_Audio: The original audio/video files are moved here after processing.

**⚠️ Important Notes**
GPU Usage: For faster transcription, ensure you have a GPU runtime enabled in Colab (Runtime > Change runtime type > GPU).
Gemini API Key: A valid Gemini API key is crucial for AI content generation. If not provided or invalid, only transcription will occur.
Supported Formats: The notebook supports .mp3, .wav, .mp4, and .m4a file formats.# AI-Transcription-Content-Generation
Automated workflow to transcribe audio/video files and generate AI-powered content based on the transcriptions.
