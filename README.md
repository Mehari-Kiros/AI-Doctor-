Project Setup Guide

This guide provides step-by-step instructions to set up your project environment, including the installation of FFmpeg and PortAudio across macOS, Linux, and Windows, as well as setting up a Python virtual environment using Pipenv, pip, or conda.
Table of Contents

    Installing FFmpeg and PortAudio
        macOS
        Linux
        Windows
    Setting Up a Python Virtual Environment
        Using Pipenv
        Using pip and venv
        Using Conda
    Running the application

Installing FFmpeg and PortAudio
macOS

Install Homebrew (if not already installed):

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

Install FFmpeg and PortAudio:

brew install ffmpeg portaudio

Linux

For Debian-based distributions (e.g., Ubuntu):

    Update the package list

sudo apt update

    Install FFmpeg and PortAudio:

sudo apt install ffmpeg portaudio19-dev

Windows
Download FFmpeg:

    Visit the official FFmpeg download page: FFmpeg Downloads
    Navigate to the Windows builds section and download the latest static build.

Extract and Set Up FFmpeg:

    Extract the downloaded ZIP file to a folder (e.g., C:\ffmpeg).
    Add the bin directory to your system's PATH:
        Search for "Environment Variables" in the Start menu.
        Click on "Edit the system environment variables."
        In the System Properties window, click on "Environment Variables."
        Under "System variables," select the "Path" variable and click "Edit."
        Click "New" and add the path to the bin directory (e.g., C:\ffmpeg\bin).
        Click "OK" to apply the changes.

Install PortAudio:

    Download the PortAudio binaries from the official website: PortAudio Downloads
    Follow the installation instructions provided on the website.

Setting Up a Python Virtual Environment
Using Pipenv

    Install Pipenv (if not already installed):

pip install pipenv

    Install Dependencies with Pipenv:

pipenv install

    Activate the Virtual Environment:

pipenv shell

Using pip and venv
Create a Virtual Environment:

python -m venv venv

Activate the Virtual Environment:

macOS/Linux:

source venv/bin/activate

Windows:

venv\Scripts\activate

Install Dependencies:

pip install -r requirements.txt

Using Conda
Create a Conda Environment:

conda create --name myenv python=3.11

Activate the Conda Environment:

conda activate myenv

Install Dependencies:

pip install -r requirements.txt

Project Phases and Python Commands
Phase 1: Brain of the doctor

python brain_of_the_doctor.py

Phase 2: Voice of the patient

python voice_of_the_patient.py

Phase 3: Voice of the doctor

python voice_of_the_doctor.py

Phase 4: Setup Gradio UI

python gradio_app.py

# AI-Doctor-
