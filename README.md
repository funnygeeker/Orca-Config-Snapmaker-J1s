# Orca-Config-Snapmaker-J1s

## 使用说明
由于 Orca Slicer 里面的 Snapmaker J1 预设在我的打印机上表现得非常糟糕，因此我花了 7 天时间对这台机器重新调整了参数，参数主要包括：

### 材料预设
PLA（使用 JAYO PLA、R3D PLA | 精细校准）
PLA Slik（基于 PLA 材料预设进行推算）
PETG（使用 Tinmorry PETG、R3D PETG | 精细校准）
TPU（使用 Tinmorry TPU | 粗略校准）
PETG-CF（基于 PETG 材料预设进行推算）
PA（基于 PA 材料预设，以及之前使用的 Bing3D PA 材料参数进行推算）
PVA（使用 PVA | 粗略校准）

### 工艺预设
- 0.16mm - Single Material
- 0.16mm - Multi Material
- 0.20mm - Single Material
- 0.20mm - Multi Material

Single Material：适用于正常的单材料打印，拥有较高的效率，可以生成正常的支撑
Multi Material：适用于使用主体材料和支撑材料打印一个模型，或者对模型进行多色打印，不过如果需要在多色打印的同时生成支撑，请将单材料参数中有关支撑的耗材参数迁移到多材料，以保持模型能被正常打印。

### 备注
- 由于 Orca 擦料塔外墙速度使用的是模型内墙速度，因此我不得不降低多材料参数的内墙打印速度以保持稳定
- 如果您需要使用多材料打印，为了材料塔不倒塌，请将擦料塔更换耗材时的冲刷量设置为 40 - 60（随高度增加，一般不超过 60，最少不建议低于 40）


## Instructions (Translation software was used, so this content may not be accurate)

Due to the poor performance of the Snapmaker J1 preset in Orca Slicer on my printer, I spent 7 days re-adjusting the parameters for this machine, including mainly:

### Material Presets
PLA (using JAYO PLA, R3D PLA | fine-tuned)
PLA Slik (based on PLA material presets)
PETG (using Tinmorry PETG, R3D PETG | fine-tuned)
TPU (using Tinmorry TPU | rough estimation)
PETG-CF (based on PETG material presets)
PA (based on PA material presets, and calculations based on previous Bing3D PA material parameters)
PVA (using PVA | rough estimation)

### Process Presets
- 0.16mm - Single Material
- 0.16mm - Multi Material
- 0.20mm - Single Material
- 0.20mm - Multi Material

Single Material: suitable for normal single material printing, with higher efficiency and capable of generating normal supports
Multi Material: suitable for printing a model using main and support materials, or for multi-color printing on a model. However, if support is needed simultaneously with multi-color printing, transfer the support-related consumable parameters from single material to multi-material to ensure the model can be printed correctly.

### Notes
- Due to Orca's wiping tower using the model's inner wall speed, I had to reduce the inner wall printing speed of the multi-material parameters to maintain stability
- If you need to use multi-material printing, to prevent the collapse of the material tower, set the purge volume when changing materials to 40 - 60 (increasing with height, generally not exceeding 60, and not recommended to be below 40)
