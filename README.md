# Orca-Config-Snapmaker-J1s
- 如果需要中文，请看最下面
- Some contents may be inaccurate using translation software.

## Instructions
Due to the poor performance of the Snapmaker J1 preset in Orca Slicer on my printer, I spent 28 days adjusting the parameters for this machine, which mainly include:

### Material presets
- PLA - PLUS (calibrated using JAYO PLA, R3D PLA)
- PLA Slik - PLUS (based on PLA material preset calculation)
- PETG - PLUS (calibrated using Tinmorry PETG, R3D PETG)
- TPU - PLUS (calibrated using Tinmorry TPU)
- PETG-CF - PLUS (calibrated using Tinmorry PETG, R3D PETG)
- PA - PLUS (based on PA material preset, and calculated based on previous Bing3D PA material parameters)
- PVA - PLUS (calibrated using PVA)

### Process presets
- 0.16mm - Single Material
- 0.16mm - Multi Material
- 0.20mm - Single Material
- 0.20mm - Multi Material

Single Material: Suitable for normal single material printing, with high efficiency and the ability to generate normal supports.

Multi Material: (specially optimized for 90-degree overhang angle) Suitable for printing a model using both main and support materials, or for multi-color printing. However, if supports are needed during multi-color printing, transfer the support-related consumable parameters from single material to multi-material to ensure the model can be printed correctly.

Multi Material 2: (specially optimized for other overhang angles, suitable for harder support materials) Suitable for printing a model using both main and support materials, or for multi-color printing. However, if supports are needed during multi-color printing, transfer the support-related consumable parameters from single material to multi-material to ensure the model can be printed correctly.

### Note
- These parameters may not be suitable for Orca V2.2.0+. Once Orva V2.2.0+ is stable, we will migrate to Orva V2.2.0+.
- Due to the use of model inner wall speed for the outer wall speed of the ooze tower in Orca V2.1.1, the inner wall print speed for multi-material parameters had to be reduced to maintain stability.
- If you need to use multi-material printing, to prevent the ooze tower from collapsing, set the wipe volume when changing consumables to 10 - 25 (increasing with height, generally not exceeding 25). Alternatively, set the wipe factor to 0 in the wipe volume multiplier to apply the minimum wipe for each consumable.
- ![image](https://github.com/user-attachments/assets/069a852a-4141-4968-9bd5-6c23eec8b397)
- Orca V2.1.1 is recommended to be used with [SM2Uploader](https://github.com/macdylan/sm2uploader/releases/tag/v2.8) for best results. Before Orca supports multi-extrusion machines, remember to use version 2.8 and set up the machine as shown in the following screenshot:
- Remember to configure parameters: `http://127.0.0.1:8899` and `-noreinforcetower;`
- ![image](https://github.com/user-attachments/assets/9462cf4b-7586-4cb4-9a5a-8a50dd7d4d38)
- When printing with different types of materials (not colors), check the support material (not the model's main material):
- ![image](https://github.com/user-attachments/assets/995dade4-bc5d-44a7-800c-a4f6fd0e4f57)
- Theoretically, these parameters can keep your device in optimal operating condition at room temperature of 22℃ - 28℃. However, at temperatures above a certain level, pay attention to cooling to prevent PETG material from curling (to maintain good overhangs, I have set the fan speed quite high, but this may have some side effects). Similarly, in winter, pay attention to whether PETG material will curl. I have not conducted experiments in winter yet, but I will update these parameters in the future.
- When the indoor temperature is 28℃ or higher, please open the top cover of the device to ensure normal printing (do not open the door, as some materials may curl).


## 使用说明
由于 Orca Slicer 里面的 Snapmaker J1 预设在我的打印机上表现得非常糟糕，因此我花了 `28` 天时间对这台机器重新调整了参数，参数主要包括：

### 材料预设
- PLA - PLUS（使用 JAYO PLA、R3D PLA 校准）
- PLA Slik - PLUS（基于 PLA 材料预设进行推算）
- PETG - PLUS（使用 Tinmorry PETG、R3D PETG 校准）
- TPU - PLUS（使用 Tinmorry TPU 校准）
- PETG-CF - PLUS（使用 Tinmorry PETG、R3D PETG 校准）
- PA - PLUS（基于 PA 材料预设，以及之前使用的 Bing3D PA 材料参数进行推算）
- PVA - PLUS（使用 PVA 校准）

### 工艺预设
- 0.12mm - Single Material
- 0.12mm - Multi Material
- 0.12mm - Multi Material 2
- 0.16mm - Single Material
- 0.16mm - Multi Material
- 0.16mm - Multi Material 2
- 0.20mm - Single Material
- 0.20mm - Multi Material
- 0.20mm - Multi Material 2

Single Material：适用于正常的单材料打印，拥有较高的效率，可以生成正常的支撑

Multi Material：（针对90度悬垂角度进行特别优化）适用于使用主体材料和支撑材料打印一个模型，或者对模型进行多色打印，不过如果需要在多色打印的同时生成支撑，请将单材料参数中有关支撑的耗材参数迁移到多材料，以保持模型能被正常打印。

Multi Material 2：（针对其他悬垂角度进行特别优化，适合比较硬的支撑材料）适用于使用主体材料和支撑材料打印一个模型，或者对模型进行多色打印，不过如果需要在多色打印的同时生成支撑，请将单材料参数中有关支撑的耗材参数迁移到多材料，以保持模型能被正常打印。

### 备注
- 该参数可能不适用于 Orca V2.2.0+，Orva V2.2.0+ 稳定后，我们将会迁移至Orva V2.2.0+
- 由于 Orca V2.1.1 擦料塔外墙速度使用的是模型内墙速度，因此我不得不降低多材料参数的内墙打印速度以保持稳定
- 如果您需要使用多材料打印，为了材料塔不倒塌，请将擦料塔更换耗材时的冲刷量设置为 10 - 25（随高度增加，一般不超过 25），当然也有更简单的方法，在冲刷体积的倍率中设置为0，即可应用各耗材的最低冲刷。
- ![image](https://github.com/user-attachments/assets/069a852a-4141-4968-9bd5-6c23eec8b397)
- Orca V2.1.1 建议搭配 [SM2Uploader](https://github.com/macdylan/sm2uploader/releases/tag/v2.8) 使用，以获得最佳效果，在 Orca 支持多挤出机之前，记住，一定要 `2.8` 版本，然后按照以下截图设置机器：
- 记得配置参数：`http://127.0.0.1:8899` 和 `-noreinforcetower;`
- ![image](https://github.com/user-attachments/assets/9462cf4b-7586-4cb4-9a5a-8a50dd7d4d38)
- 使用不同类型的材料打印时（不同颜色的不需要），请在支撑材料处勾选（模型主体材料不需要）：
- ![image](https://github.com/user-attachments/assets/995dade4-bc5d-44a7-800c-a4f6fd0e4f57)
- 理论上这一套参数可以供你的设备在室温 `22℃` - `28℃` 保持最佳的运行状态，不过高于一定温度时，您需要注意散热，散热时应当特别注意 `PETG` 材料是否会翘起（为了保持良好的悬垂，风扇我开的比较大，但是这可能会带来一些副作用），冬天时同样也应当注意 `PETG` 材料是否会翘起，目前我并没有在冬天做过实验，我会在后续更新这些参数。
- 当室内温度超过或等于 `28℃` 时，请打开设备的顶盖，以保持正常打印（不要开门，否则部分材料可能会翘起）。
