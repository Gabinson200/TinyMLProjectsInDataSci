# TinyMLProjectsInDataSci
Repository for code containing models, code, and visualization for tinyML projects in data science

The TFLM_speech_model.ipynb and Adam_k_gAItor_KeywordSpotting.ipynb colabs were my first exploration and experimentation with building CNNs on audio data as I have never used such data in the past.
The project_in_data_sci_visu.ipynb colab was used to create visualizations from the data gathered during mode creation and evaluation.
The to_cc_file_converter.ipynb converts different file types to .cc so that they can be uploaded to MCUs.

The models, converted_models, and converted_wav_files folders hold all of the model data including pictures of architecture, training error and checkpoint data, and necessary MCU ready conversions of files made by the to_cc_file_converter.ipynb colab.


The Arduino Folder contains the two different versions of the hardware code with  micro_speech_ported one based on the Espressif version of the new code which was in turn based on the original Arduino code in the micro_speech_adam_version_old. For more information on these files consult the READ.ME in the Arduino folder.

While I had to port the TFLM library to work with my Windows machine using MSVC I only included the Linux version of the modified TFLM micro speech example which this project is based from because getting the code to work on my machine required much more device-specific setup than I can document here. Furthermore, the building of TFLM from a source using Linux is by far the superior option. Please consult the LinuxMicro Speech folder on how to set up the additionally created tests.
