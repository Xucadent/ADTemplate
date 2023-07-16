# ADTemplate

ADTemplate包含了一组Altium Designer软件自定义配置所需的文件，包括常用的2层和4层PCB工程模板、PCB视图配置、优选项配置和快捷键配置，具体如下：

- `DraftView.config_complex`：PCB元素完全以轮廓显示(Draft)的2D视图配置和配色接近真实的黑色阻焊PCB 3D视图配置。
- `DXP.RCS`：按照立创EDA和一些常用操作英文名称设定的快捷键配置。
- `LowSaturation.PCBSysColors`：一组低饱和度的PCB图层配色。
- `Preferences.DXPPrf`：优选项配置。
- `backup`：PCB工程模板使用的图层组合(.layerset)、层压结构(.stackup)、规则(.RUL)。
- `PCB_2(4)Layer_Template`：PCB工程模板，包括工程文件、原理图、PCB文档、输出配置文件。

对于未列出的细节，可以参考[Altium Designer自定义和工程模板](https://flickerz.xyz/p/rm%E7%A1%AC%E4%BB%B602-altium-designer%E8%87%AA%E5%AE%9A%E4%B9%89%E5%92%8C%E5%B7%A5%E7%A8%8B%E6%A8%A1%E6%9D%BF%E6%96%BD%E5%B7%A5%E4%B8%AD/)

## 快速配置

1. 点击右上角的优选项设置![icon1](https://github.com/Xucadent/ADTemplate/blob/main/docs/icon1.png)，选择`加载->从文件中加载`，打开`Preferences.DXPPrf`，等待导入完成后关闭Altium Designer。
2. 使用Windows的资源管理器打开`%USERPROFILE%\AppData\Roaming\Altium`，在此目录下打开`Altium Designer {xxx}`(xxx是一个不固定的字符串)文件夹，将`DXP.RCS`粘贴到此处。再打开`ViewConfigurations`文件夹，将`DraftView.config_complex`和`LowSaturation.PCBSysColors`粘贴到此处。
3. 打开Altium Designer，再次进入优选项设置，在`PCB Editor -> Layer Colors`中选择**载入颜色配置文件**，打开`LowSaturation.PCBSysColors`。
4. 注册并登录[DigiPCBA](https://space.digipcba.com/signup)，创建Workspace。如有团队工作账号请登**团队账号**并打开Workspace并**跳转到第5步**。点击右下角的![icon2](https://github.com/Xucadent/ADTemplate/blob/main/docs/icon2.png)打开Explorer，并在适当位置**创建**Project Template项目，完成后在其右键菜单的Upload选项中选择`PCB_2(4)Layer_Template`文件夹中的.PrjPcb工程上传。
5. 选择`文件->新的->PCB`(无需保存)，点击右下角的![icon2](https://github.com/Xucadent/ADTemplate/blob/main/docs/icon2.png)打开View Configuration，打开View Options选项卡后，选择`General Settings -> Configuration`的下拉菜单中最后一项Load View Configuration并打开`DraftView.config_complex`，此时下拉菜单中出现DraftView配置，选择之后将下方的Mask and Dim Settings三项分别拖动至(40%/40%/80%)，设置完成。

