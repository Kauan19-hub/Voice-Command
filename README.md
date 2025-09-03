**<h2>💻 Código do Áudio Desenvolvido em Python 💻</h2>**

###
```python
import edge_tts as ets
import asyncio

async def text_audio(text, name_of_archive):
    voice = "pt-BR-AntonioNeural"
    tts = ets.Communicate(text, voice)
    
    print("Áudio está sendo gerado...")
    await tts.save(name_of_archive)

    print(f'Áudio salvo como {name_of_archive}')

def main():
    text = """
    Com essa função, você pode converter qualquer texto, para voz do Google!
    """

    name_of_archive = "txt_audio.mp3"
    asyncio.run(text_audio(text, name_of_archive))

if __name__ == '__main__':
    main()
```

###

Um código simples em Python, tem como função, converter qualquer tipo de texto, em áudio `mp3` com voz do próprio Google!<br>
Para isso, é necessário baixar livrarias/frameworks para importar a função que permite o usuário a realizar o código.

###

(**OBS**: Dependendo da voz que você utilizar, precisa instalar outra biblioteca/framework, e será necessário verificar se sua máquina<br>
possui a voz que você escolheu. Cada sistema ou navegador, possui suas próprias vozes do Google! 😉

---

Espero que goste! Caso queira testá-lo, poderá copiar este código, baixar o áudio `mp3` acima, clique em `view raw` e seguir os requisitos necessários: ⬇️

###

**<h3>✅ Ambiente Virtual (Terminal do VS Code)</h3>**

###

Para Windows:

###
```powershell
python -m venv env  #Cria o ambiente
.\env\Scripts\activate #Entra no ambiente
```
###

Para Linux:

###
```powershell
$ mkdir (nome...)
$ python3 -m venv venv
```

###

Para MacOS:

###
```powershell
pip3 -m venv env (name...)
pip3 -m venv env (name...) activate
pip install (nome do pacote...) #Caso queira instalar pacotes específios
```

###

😎 Seguindo esse passo, você criará uma `env` dentro de seu VS Code. Caso queira usar a mesma dependência que usei no código, instale:

###
```powershell
pip install edge_tts
```

###

**<h3>🗣️ Voz utilizada no código</h2>**

###
```python
 voice = "pt-BR-AntonioNeural"

 #PT-BR or EN
```
