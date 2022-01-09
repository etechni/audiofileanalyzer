# audiofileanalyzer
Analyze the following speech quality indicators like repetition of words,pauses, using existing APIs, libraries
Datascience Tasks
The task consist of a voice note of 2 speakers. The goal is to analyse the speech using the following questions given:
1) Count the number of pauses 
2) Count the repetition of words 
3) Count the number of different words used 
4) Number of words spoken per minute 
5) Count number of “aaaa
Step 1: Heard the audio file to understand the type of file song or speech, check the files’s clarity.
Step2: Imported required libraries to work with audio file. SpeechRecognition library helps in recognizing speech. To analyse count number of words and its repetition, audio is converted to text using pydub library. Since audio file is large we split into smaller files to transcribe from google speech recognition. Combine the text in string variable audioTranscript.
Step3: 
Q3. To count number of different words, list is created to store words as listWords. Using numpy library will give unique words from the list.
Q2.Count the frequency of words: check the repetition of words in listWords, if word is present increment count by 1, else add to dictionary with count 1.  A dictionary is initialised to store words and its count.
Q3. Count number of pauses: In a conversation, there are different levels of decibels. Hence, a change in sound levels.  We give threshold dbfs value to detect pauses in audio. Pydub library is used to detect silences in audio. Threshold value of -100 db is taken for length of 1 second and creates number of chunks to give number of pauses of length 1 second.
