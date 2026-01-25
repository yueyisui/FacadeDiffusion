# Datasets

This project assumes **paired façade images and semantic maps**.

## Expected directory layout (example)

```
data/
  train/
    images/
      image.png
    labels/
      semantic.png
    prompts/
      prompt.txt
  test/
    images/
      image.png
    labels/
      semantic.png
    prompts/
      prompt.txt
```

## Label convention
- You may store semantic maps as:
  - integer label PNG (recommended), or
  - color-coded PNG (ensure a fixed palette mapping).

## LSAA-v2 license statement (copy/paste)

> The [LSAA dataset](https://github.com/ZPdesu/lsaa-dataset?tab=readme-ov-file) is a derivative work based on the LSAA dataset, with additional semantic annotations created by the authors.  
> In accordance with the original license, LSAA-v2 is released under the [Creative Commons BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) license.
