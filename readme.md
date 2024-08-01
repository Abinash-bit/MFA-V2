# Auto-Subtitling for Indian Languages.

As part of the [BIRD](https://billionreaders.org/) initiative , we aim to create a tool which can speed up the adoption of Same Language Subtitling (SLS) among the content producers for the entire country.
This will ensure that 200M weak readers and 30M readers with accessibility to get regular reading exposure with content having SLS.

This tool will create SRT files by taking a video file and its text file.
We aim for the tool to support the following languages : English, Hindi, Tamil and Punjabi for now.

## Replicating the Development Environment

These instructions will give you a copy of the project up and running on
your local machine for development and testing purposes. See deployment
for notes on deploying the project on a live system.

### Prerequisites

Requirements for the software and other tools to build, test and push 
- Windows 11 64-bit
- Lower version of windows also works fine

### Installing

A step by step series of examples that tell you how to get a development
environment running

[Download Miniconda3](https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.exe/)

Navigate through the installation Steps in Windows Just Click on Next.
Open miniconda3 prompt in Windows and check the conda version

    conda --version
    #24.5.0

Create a Working Directory

    mkdir ASP-project
    cd ASP-project

Install Montreal Force Aligner

    conda create -n aligner -c conda-forge montreal-forced-aligner
    conda activate aligner

Install Pytorch CPU

    conda install pytorch torchvision torchaudio cpuonly -c pytorch

Install SpeechBrain

    pip install speechbrain    


Inside the aligner conda environment install python libraries

    pip install pysrt streamlit aksharamukha moviepy
    


## Running the tests

Download the pretrained models from google drive [link](https://drive.google.com/drive/folders/1tKWAEtgFSK5pngsP08mYECbLaH4-_ROt?usp=sharing)
This link will contain two extra folders named "forced_alignment" and "upload" download these two also they handle file handling temporarily.
Store them in the working directory you have created.

Inside the working directory 

    git clone 


### Sample Tests

Explain what these tests test and why

    Give an example

### Style test

Checks if the best practices and the right coding style has been used.

    Give an example

## Deployment

Add additional notes to deploy this on a live system

## Built With

  - [Contributor Covenant](https://www.contributor-covenant.org/) - Used
    for the Code of Conduct
  - [Creative Commons](https://creativecommons.org/) - Used to choose
    the license

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code
of conduct, and the process for submitting pull requests to us.

## Versioning

We use [Semantic Versioning](http://semver.org/) for versioning. For the versions
available, see the [tags on this
repository](https://github.com/PurpleBooth/a-good-readme-template/tags).

## Authors

  - **Billie Thompson** - *Provided README Template* -
    [PurpleBooth](https://github.com/PurpleBooth)

See also the list of
[contributors](https://github.com/PurpleBooth/a-good-readme-template/contributors)
who participated in this project.

## License

This project is licensed under the [CC0 1.0 Universal](LICENSE.md)
Creative Commons License - see the [LICENSE.md](LICENSE.md) file for
details

## Acknowledgments

  - Hat tip to anyone whose code is used
  - Inspiration
  - etc

