# Orca-Config-Snapmaker-J1s
- 如果需要中文，请看最下面
- Some contents may be inaccurate using translation software.

## Instructions

Since the Snapmaker J1 preset in Orca Slicer performs very poorly on my printer, I spent about `60` days re-adjusting the parameters for this machine. The adjustments mainly include:

### Bug Fixes
- Added an additional temperature range during preheating to fix a bug where certain G-Code commands were skipped by the printer firmware in specific material print sequences.

### Material Presets
![image](https://github.com/user-attachments/assets/56c005a4-8b8d-44dd-970a-13b71157c6a8)

### Process Presets
![image](https://github.com/user-attachments/assets/522f2a30-d196-4d0b-9baf-2057484099e6)
- `XXXX - Brass` refers to the material specifications of the brass nozzle pre-installed on the machine at the time of factory shipment.
![image](https://github.com/user-attachments/assets/33b67d68-3a81-4bf2-bd8b-28b359f2de49)
- `XXXX - Hardened Steel` refers to the material specifications of the machine's new version of the hardened steel nozzle.
![image](https://github.com/user-attachments/assets/64e113b5-b073-4394-b546-4e749583425e)

**Same Material**: Suitable for printing with the same type of material. It provides high efficiency and generates normal supports.

**PVA Support**: Print parameters specifically optimized for PVA water-soluble material.

**Plane Support**: (Specially optimized for 90-degree overhang angles) Suitable for printing a model using both main and support materials.

**Curved Support**: (Optimized for other overhang angles, suitable for harder support materials) Suitable for printing a model using both main and support materials.

### Notes
- These parameters may not be compatible with Orca V2.1.0 or earlier versions.
- ![image](https://github.com/user-attachments/assets/069a852a-4141-4968-9bd5-6c23eec8b397)
- Orca V2.2.0 is recommended to be used with [SM2UploaderV2.9](https://github.com/macdylan/sm2uploader/releases/tag/v2.9) for optimal performance. Before Orca supports multiple extruders, remember to use version `2.9` and configure the machine settings as shown in the following screenshots:
- Don't forget to configure the parameter: `http://127.0.0.1:8899`
- ![image](https://github.com/user-attachments/assets/9462cf4b-7586-4cb4-9a5a-8a50dd7d4d38)
- When printing with different types of materials (different colors are not needed), check the box for the support material (the main model material does not require this):
- ![image](https://github.com/user-attachments/assets/995dade4-bc5d-44a7-800c-a4f6fd0e4f57)
- In theory, this set of parameters allows your device to maintain optimal operating conditions in room temperatures between `22°C` and `28°C`. However, if the temperature exceeds a certain level, you need to be cautious about cooling. Pay special attention to whether the `PETG` material warps when cooling (I keep the fan speed relatively high to ensure good overhangs, but this might have some side effects). During the winter, you should also monitor whether `PETG` warps.
- When the indoor temperature reaches or exceeds `28°C`, please open the top cover of the device to ensure normal printing (do not open the door, as some materials might warp).
- (This device has already been sold by me, and the parameters will not be updated later.)

## 使用说明
由于 Orca Slicer 里面的 Snapmaker J1 预设在我的打印机上表现得非常糟糕，因此我花了约 `60` 天时间对这台机器重新调整了参数，参数主要包括：

### 错误修复
- 预热时增加了一个额外的温度区间，修复了在某些特定的材料打印顺序下，部分 G-Code 代码会被打印机固件异常跳过的 BUG。

### 材料预设
![image](https://github.com/user-attachments/assets/56c005a4-8b8d-44dd-970a-13b71157c6a8)


### 工艺预设
![image](https://github.com/user-attachments/assets/522f2a30-d196-4d0b-9baf-2057484099e6)
- `XXXX - Brass` 指机器出厂时预装的黄铜喷嘴的材料参数。
- ![image](https://github.com/user-attachments/assets/33b67d68-3a81-4bf2-bd8b-28b359f2de49)
- `XXXX - Hardened Steel` 指机器的新版硬化钢喷嘴的材料参数。
![image](https://github.com/user-attachments/assets/64e113b5-b073-4394-b546-4e749583425e)

Same Material：适用于相同种类的材料打印，拥有较高的效率，可以生成正常的支撑。

PVA Support：针对 PVA 水溶性材料特别优化的打印参数。

Plane Support：（针对90度悬垂角度进行特别优化）适用于使用主体材料和支撑材料打印一个模型。

Curved Support：（针对其他悬垂角度进行特别优化，适合比较硬的支撑材料）适用于使用主体材料和支撑材料打印一个模型。

### 备注
- 该参数可能不适用于 Orca V2.1.0 或早期版本。
- ![image](https://github.com/user-attachments/assets/069a852a-4141-4968-9bd5-6c23eec8b397)
- Orca V2.2.0 建议搭配 [SM2UploaderV2.9](https://github.com/macdylan/sm2uploader/releases/tag/v2.9) 使用，以获得最佳效果，在 Orca 支持多挤出机之前，记住，一定要 `2.9` 版本，然后按照以下截图设置机器：
- 记得配置参数：`http://127.0.0.1:8899`
- ![image](https://github.com/user-attachments/assets/9462cf4b-7586-4cb4-9a5a-8a50dd7d4d38)
- 使用不同类型的材料打印时（不同颜色的不需要），请在支撑材料处勾选（模型主体材料不需要）：
- ![image](https://github.com/user-attachments/assets/995dade4-bc5d-44a7-800c-a4f6fd0e4f57)
- 理论上这一套参数可以供你的设备在室温 `22℃` - `28℃` 保持最佳的运行状态，不过高于一定温度时，您需要注意散热，散热时应当特别注意 `PETG` 材料是否会翘起（为了保持良好的悬垂，风扇我开的比较大，但是这可能会带来一些副作用），冬天时同样也应当注意 `PETG` 材料是否会翘起。
- 当室内温度超过或等于 `28℃` 时，请打开设备的顶盖，以保持正常打印（不要开门，否则部分材料可能会翘起）。
- （这个机子已经被我卖掉了，后续不会再更新参数了）
