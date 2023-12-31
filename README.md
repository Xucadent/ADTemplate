# ADTemplate

ADTemplate包含了一组Altium Designer软件自定义配置所需的文件，包括常用的2层和4层PCB工程模板、PCB视图配置、优选项配置和快捷键配置，具体如下：

- `Preferences.DXPPrf`：优选项配置。
- `PCBEditorDefault_InvertedText.dft`：带有丝印文本反白效果的PCB编辑器配置文件。
- `backup`：PCB工程模板使用的图层组合(.layerset)、层压结构(.stackup)、规则(.RUL)、低饱和度PCB图层配色(.PCBSysColors)、快捷键配置(.RCS)、PCB视图配置(.config_complex)。
- `PCB_2(4)Layer_Template`：PCB工程模板，包括工程文件、原理图、PCB文档、输出配置文件。

对于未列出的细节，可以参考[Altium Designer自定义和工程模板](https://flickerz.xyz/p/rm%E7%A1%AC%E4%BB%B602-altium-designer%E8%87%AA%E5%AE%9A%E4%B9%89%E5%92%8C%E5%B7%A5%E7%A8%8B%E6%A8%A1%E6%9D%BF%E6%96%BD%E5%B7%A5%E4%B8%AD/)

## 快速配置

1. 点击右上角的优选项设置![icon1](https://github.com/Xucadent/ADTemplate/blob/main/docs/icon1.png)，选择`加载->从文件中加载`，打开`Preferences.DXPPrf`，等待导入完成后关闭Altium Designer。
3. 打开Altium Designer，再次进入优选项设置，在`PCB Editor -> Layer Colors`中选择**载入颜色配置文件**，打开`LowSaturation.PCBSysColors`并应用，如果需要[打开丝印文本反白效果](https://www.altium.com/documentation/altium-designer/nfs-20-0pcb-text-string-improvements-ad?version=20.0)（第一个图），在`PCB Editor -> Defaults -> String`中点击中间下方的Load然后打开`PCBEditorDefault_InvertedText.dft`并应用（导入第二次打开才能正常显示）。
4. 注册并登录[DigiPCBA](https://space.digipcba.com/signup)，创建Workspace。如有团队工作账号请登**团队账号**并打开Workspace，**跳转到第4步**。点击右下角的![icon2](https://github.com/Xucadent/ADTemplate/blob/main/docs/icon2.png)打开Explorer，并在适当位置**创建**Project Template项目，完成后在其右键菜单的Upload选项中选择`PCB_2(4)Layer_Template`文件夹中的.PrjPcb工程上传。
5. 选择`文件->新的->PCB`(无需保存)，点击右下角的![icon2](https://github.com/Xucadent/ADTemplate/blob/main/docs/icon2.png)打开View Configuration，打开View Options选项卡后，选择`General Settings -> Configuration`的下拉菜单中最后一项Load View Configuration并打开`DraftView.config_complex`，此时下拉菜单中出现DraftView配置，选择之后将下方的Mask and Dim Settings三项分别拖动至(40%/40%/80%)，设置完成。

