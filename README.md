<h2>Audio Code Developed in Python</h2>

###
```python
import edge_tts as ets
import asyncio

async def text_audio(text, name_of_archive):
    voice = "pt-BR-AntonioNeural"
    tts = ets.Communicate(text, voice)
    
    print("Audio is being generated...")
    await tts.save(name_of_archive)

    print(f'Audio saved as {name_of_archive}')

def main():
    text = """
    With this function, you can convert any text to Google voice!
    """

    name_of_archive = "txt_audio.mp3"
    asyncio.run(text_audio(text, name_of_archive))

if __name__ == '__main__':
    main()
```

###

A simple code in Python, its function is to convert any type of text into `mp3` audio with Google's own voice!
For this, it is necessary to download libraries/frameworks to import the function that allows the user to execute the code.


###


(OBS: Depending on the voice you use, you need to install another library/framework, and you will need to check if your machine
has the voice you have chosen. Each system or browser has its own Google voices!

---

Hope you like it! If you want to test it, you can copy this code, download the `mp3` audio above, click on `view raw` and follow the necessary requirements: ⬇️

###

**<h3>✅ Virtual Environment (VS Code Terminal)</h3>**

###

For Windows:

###
```powershell
python -m venv env  #Creates the environment
```

###
```powershell
.\env\Scripts\activate #Enters the environment
```

###

For Linux:

###
```powershell
$ mkdir (name...)
```

###
```powershell
$ python3 -m venv venv
```

###

For MacOS:

###
```powershell
pip3 -m venv env (name...)
```

###
```powershell
pip3 -m venv env (name...) activate
```

###
```powershell
pip install (package name...) #If you want to install specific packages
```

###

Following this step, you will create an `env` inside your VS Code. If you want to use the same dependency that I used in the code, install:

###
```powershell
pip install edge_tts
```

###

**<h3>🗣️ Voice used in the code</h2>**

###
```python
 voice = "pt-BR-AntonioNeural"

 #PT-BR or EN
```
