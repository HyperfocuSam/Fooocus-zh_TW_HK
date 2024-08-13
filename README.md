# Fooocus-zh_TW_HK
Fooocus 繁體中文翻譯介面 | Traditional Chinese UI translation for Fooocus



---

##Update Logs

- Updated 13-08-2024

Translation completed. Translated text upon manual review and finetune.  

- Updated 12-08-2024

Original repository : https://github.com/lllyasviel/Fooocus/tree/main ; v2.5.5, release date 12/08/2024

Translation mainly powered by Claude 3 Opus. Will be followed by manual review and fine-tune.

## Setting up | Translated instruction 

您可以將json文件放在language文件夾中以翻譯用戶界面。

例如，下面是Fooocus/language/example.json的內容：

```json
{
  "Generate": "生成",
  "Input Image": "輸入圖像",
  "Advanced": "高級",
  "SAI 3D Model": "SAI 3D模型"
}
```

如果您添加 "--language example" 參數，Fooocus將讀取Fooocus/language/example.json來翻譯UI。

例如，您可以將`Windows run.bat`的結尾行編輯為

`.\python_embeded\python.exe -s Fooocus\entry_with_update.py --language example`

或將`run_anime.bat`編輯為

`.\python_embeded\python.exe -s Fooocus\entry_with_update.py --language example --preset anime`

或將`run_realistic.bat`編輯為

`.\python_embeded\python.exe -s Fooocus\entry_with_update.py --language example --preset realistic`


- Instruction from original repository by lllyasviel

## Localization/Translation/I18N

You can put json files in the `language` folder to translate the user interface.

For example, below is the content of `Fooocus/language/example.json`:

```json
{
  "Generate": "生成",
  "Input Image": "入力画像",
  "Advanced": "고급",
  "SAI 3D Model": "SAI 3D Modèle"
}
```

If you add `--language example` arg, Fooocus will read `Fooocus/language/example.json` to translate the UI.

For example, you can edit the ending line of Windows `run.bat` as

    .\python_embeded\python.exe -s Fooocus\entry_with_update.py --language example

Or `run_anime.bat` as

    .\python_embeded\python.exe -s Fooocus\entry_with_update.py --language example --preset anime

Or `run_realistic.bat` as

    .\python_embeded\python.exe -s Fooocus\entry_with_update.py --language example --preset realistic

For practical translation, you may create your own file like `Fooocus/language/jp.json` or `Fooocus/language/cn.json` and then use flag `--language jp` or `--language cn`. Apparently, these files do not exist now. **We need your help to create these files!**

Note that if no `--language` is given and at the same time `Fooocus/language/default.json` exists, Fooocus will always load `Fooocus/language/default.json` for translation. By default, the file `Fooocus/language/default.json` does not exist.