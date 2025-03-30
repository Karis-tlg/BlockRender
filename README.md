# Block Icon Render Action  

This action generates isometric block icons for Minecraft using textures from a specified directory. It is based on the [cubeSpriteGenerator](https://github.com/ofunny/ofunnysBedrockExamples/tree/main/cubeSpriteGenerator) project by [ofunny](https://github.com/ofunny).  

## Requirements  
- [ImageMagick](https://imagemagick.org/) (Ensure "convert" is included during installation)  
- Bash (Linux, macOS, or Windows WSL)  

# Usage:
 - 1. Go to the "Actions" tab in your GitHub repository.
 - 2. Select "Render Block" from the list of workflows.
 - 3. Click "Run workflow" and enter the URL to the textures zip file.
 - 4. The generated icons will be available as an artifact named "Icon".

## Usage  
Run the script with:  
```bash
bash ./convert.sh [input_directory] [output_directory]
```  
Example:  
```bash
bash ./convert.sh input/ output/
```  

### Custom Block Sides  
To specify different textures for cube sides, add suffixes to the filenames:  
- `_top` → Top side  
- `_north` → Front side  
- `_west` → Left side  

Example files:  
```
andesite_pillar.png  
andesite_pillar_top.png  
andesite_pillar_north.png  
andesite_pillar_west.png  
```  

## Credits  
This project is based on [cubeSpriteGenerator](https://github.com/ofunny/ofunnysBedrockExamples/tree/main/cubeSpriteGenerator) by [ofunny](https://github.com/ofunny). Please respect the original license.