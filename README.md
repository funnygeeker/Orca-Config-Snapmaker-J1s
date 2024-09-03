# Orca-Config-Snapmaker-J1s

## 使用说明
由于 Orca Slicer 里面的 Snapmaker J1 预设在我的打印机上表现得非常糟糕，因此我花了 `7 + 14` 天时间对这台机器重新调整了参数，参数主要包括：

### 材料预设
- PLA - PLUS（使用 JAYO PLA、R3D PLA 校准）
- PLA Slik - PLUS（基于 PLA 材料预设进行推算）
- PETG - PLUS（使用 Tinmorry PETG、R3D PETG 校准）
- TPU - PLUS（使用 Tinmorry TPU 校准）
- PETG-CF - PLUS（使用 Tinmorry PETG、R3D PETG 校准）
- PA - PLUS（基于 PA 材料预设，以及之前使用的 Bing3D PA 材料参数进行推算）
- PVA - PLUS（使用 PVA 校准）

### 工艺预设
- 0.16mm - Single Material
- 0.16mm - Multi Material
- 0.20mm - Single Material
- 0.20mm - Multi Material

Single Material：适用于正常的单材料打印，拥有较高的效率，可以生成正常的支撑

Multi Material：适用于使用主体材料和支撑材料打印一个模型，或者对模型进行多色打印，不过如果需要在多色打印的同时生成支撑，请将单材料参数中有关支撑的耗材参数迁移到多材料，以保持模型能被正常打印。

### 备注
- 由于 Orca 擦料塔外墙速度使用的是模型内墙速度，因此我不得不降低多材料参数的内墙打印速度以保持稳定
- 如果您需要使用多材料打印，为了材料塔不倒塌，请将擦料塔更换耗材时的冲刷量设置为 10 - 25（随高度增加，一般不超过 25）
- ![image](https://github.com/user-attachments/assets/069a852a-4141-4968-9bd5-6c23eec8b397)
- Orca V2.1.1 建议搭配 [SM2Uploader](https://github.com/macdylan/sm2uploader/releases/tag/v2.8) 使用，以获得最佳效果，在 Orca 支持多挤出机之前，记住，一定要 `2.8` 版本，然后按照以下截图设置机器：
- 记得配置参数：`http://127.0.0.1:8899` 和 `-noreinforcetower;`
- 使用不同的材料打印时，请在支撑材料处勾选（模型主体材料不需要）：
- ![image](https://github.com/user-attachments/assets/9462cf4b-7586-4cb4-9a5a-8a50dd7d4d38)
- 理论上这一套参数可以供你的设备在室温 `22℃` - `28℃` 保持最佳的运行状态，不过高于一定温度时，您需要注意散热，散热时应当特别注意 `PETG` 材料是否会翘起（为了保持良好的悬垂，风扇我开的比较大，但是这可能会带来一些副作用），冬天时同样也应当注意 `PETG` 材料是否会翘起，目前我并没有在冬天做过实验，我会在后续更新这些参数。


## Instructions (Translation software was used, so this content may not be accurate)

## Instructions
Due to the poor performance of the Snapmaker J1 preset in Orca Slicer on my printer, I spent `7 + 14` days readjusting the parameters for this machine, mainly including:

### Material Presets
- PLA - PLUS (calibrated using JAYO PLA, R3D PLA)
- PLA Slik - PLUS (calculated based on PLA material presets)
- PETG - PLUS (calibrated using Tinmorry PETG, R3D PETG)
- TPU - PLUS (calibrated using Tinmorry TPU)
- PETG-CF - PLUS (calibrated using Tinmorry PETG, R3D PETG)
- PA - PLUS (based on PA material presets and calculations from previous Bing3D PA material parameters)
- PVA - PLUS (calibrated using PVA)

### Process Presets
- 0.16mm - Single Material
- 0.16mm - Multi Material
- 0.20mm - Single Material
- 0.20mm - Multi Material

Single Material: suitable for normal single material printing with higher efficiency, capable of generating normal supports

Multi Material: suitable for printing a model using main and support materials, or for multi-color printing on a model. If support is needed simultaneously with multi-color printing, transfer support-related consumable parameters from single material to multi-material for the model to be printed correctly.

### Notes
- Due to Orca using the model's inner wall speed in the wiping tower's outer wall speed, I had to lower the inner wall printing speed of the multi-material parameters to maintain stability
- If you need to use multi-material printing, to prevent the collapse of the material tower, set the purge volume when changing materials to 10 - 25 (increasing with height, generally not exceeding 25)
- ![image](https://github.com/user-attachments/assets/069a852a-4141-4968-9bd5-6c23eec8b397)
- Orca V2.1.1 recommends using [SM2Uploader](https://github.com/macdylan/sm2uploader/releases/tag/v2.8) for optimal results. Before Orca supports multi-extrusion machines, remember to use version `2.8`, then set up the machine according to the screenshot below:
- Remember to configure the parameters: `http://127.0.0.1:8899` and `-noreinforcetower;`
- When printing with different materials, select support materials (the main material of the model does not need this):
- ![image](https://github.com/user-attachments/assets/9462cf4b-7586-4cb4-9a5a-8a50dd7d4d38)
- In theory, this set of parameters can keep your device in optimal condition at room temperature `22℃` - `28℃`. However, at temperatures above a certain threshold, ensure proper heat dissipation. Pay particular attention to whether the `PETG` material will warp (for good overhangs, I use a large fan, but this may have some side effects). Similarly, in winter, watch for `PETG` warping. I have not experimented in winter yet, and I will update these parameters later.
