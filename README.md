# Auto-GPT-Translator

This code intends to be a universal translator that accepts any file and uses the power of LLMs (particularly GPT for now) to translate any given text into any given language, including not only `.txt` files, but also `.tex`, `.html`, `.md` and any code in general. Support for `.doc` files is underway and `.pdf` as well, though this is trickier.

## How to use

Create a `.env` file and put your OpenAI API key like this:

```
OPENAI_API_KEY=xxxxxxx
```

In order to use the translator, just run

```
python main.py path_to_file -m gpt-3.5-turbo -lan english
```

and the processing will begin. A file with the same name `-translated` will be created in the current directory.
