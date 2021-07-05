How to use Colab:
- You will need a gmail account
- You might need a GitHub account.


1. Go to https://colab.research.google.com/notebooks/intro.ipynb?utm_source=scs-index#recent=true
2. Go to the GitHub tab and paste: https://github.com/bordeaux-neurocampus/CNCC-2021-beginner
3. You should see all the notebooks now, choose the one you want to work on.
4. Save a copy in your own Drive (File > Save a copy in Drive).
5. Work on your copy, that's your file now.
6. For those working on the project via Colab, another step is important [Mount your Data](https://colab.research.google.com/notebooks/io.ipynb)
- We recommend you to upload the dataset to your Google Drive.
- Then you'll have to follow [this](https://colab.research.google.com/notebooks/io.ipynb#scrollTo=u22w3BFiOveA). Basically, you'll have to add the following code snippet to your notebook:
     ```python
      from google.colab import drive
      drive.mount('/content/drive')
     ```
 - Then, you'll have to change the path to find the files, accordingly, e.g.:
      ```python
      filename = "/content/drive/MyDrive/records/record-001.wav"
      ```
