# G-Wolves-Open-Source-Code-Wireless-Mouse
English：
G-Wolves-Open-Source-Code-Wireless-Mouse
 Just for G-Wolvese Open Source Wireless Mouse
★How to buy:
https://shop.g-wolves.com/products/g-wolves-hati-s-open-source-wireless-mouse-58g-senseor-3370
★Important Notice:
Exercise extreme caution when updating the mouse firmware, as improper updates can render the mouse unusable. Be sure to perform a simulation test of the mouse firmware code before proceeding with the firmware update.

1. Links to technical documentation References:
English:
http://developer.nordicsemi.com/nRF_Connect_SDK/doc/1.6.0/nrf/applications/nrf_desktop/README.html
Chinese: (Chinese)
https://www.cnblogs.com/iini/p/14174427.html
2. Build compilation environment:
1) Install nrfconnect-setup-3.7.0-ia32.exe, and then find the toolchain manager under the app interface. For the attacks that need to be installed, please refer to the manual or install them all.
2) After running the toolchain manager, refer to the documents, reference links and relevant web pages to download sdkv1 6.0 or sdkv1 7.0。
3) You can also refer to the above technical documents in English or Chinese, which describes how to install SDK packages. You can directly use the NCS provided by us_ v1. 6.0. Rar file, build the compilation environment according to the instructions of the reference technical documents.
4）SDK v1. After the compilation environment of 60 is ready, you can start the compilation of the program.
5) Run SDK v1 6 compiler, select Open NRF connect SDK project and select the corresponding project:
Projects：nrf_ desktop
Board name mouse corresponds to nrf52840gmouse_ nrf52840, 
Dongle corresponds to nrf52840dongle_ nrf52840，
Default to other.
Very important: for extra cmake build option, please refer to the link above and fill in -DCMAKE_BUILD_TYPE=ZReleaseB0. Only in this way can you switch to. You can update the release version of firmware online.
6) After the project file is compiled, it is displayed in NRF_ There is a corresponding directory under the desktop (e.g. build_nrf52840gmouse_nrf52840\zephyr). Find dfu_application.zip, overwriting the corresponding dongle or mouse_dfu_release/configurator_cli the corresponding file under this folder.
7) Firmware update tool using dongle_ dfu_release And mouse_ dfu_release Batch files in the directory of.

中文説明：
G-Wolves開源固件無綫鼠標

★購買鏈接：https://g-wolves.cn/products/g-wolves-hati-s-open-source-wireless-mouse-58g-senseor-3370

★重要提示：在更新鼠标固件时务必要谨慎，否则可能导致鼠标无法使用，也無法恢復。请务必先对鼠标固件代码进行模拟测试，然后再执行固件更新。

1、技术资料文档参考的链接：
English:
http://developer.nordicsemi.com/nRF_Connect_SDK/doc/1.6.0/nrf/applications/nrf_desktop/README.html
Chinese:（中文）
https://www.cnblogs.com/iini/p/14174427.html

2、编译环境搭建：

1）安装nrfconnect-setup-3.7.0-ia32.exe，然后在app的界面下找到Toolchain Manager。需要安装的攻击，请看说明书，或者全部都安装。

2）运行Toolchain Manager后，参考文档参考链接和相关网页，下载SDKv1.6.0或SDKv1.7.0。

3）你也可以参考英文或者中文的上述技术文档，上面介绍了如何安装SDK程序包。可以直接使用我们提供的ncs_v1.6.0.rar文件，按照参考技术文档的说明，进行编译环境搭建。

4）SDK v1.60的编译环境准备好之后，就可以开始程序的编译。

5）运行SDK v1.6的编译器，选择open nrf connect sdk project，选择对应项目即可：

Projects：nrf_desktop
Board Name鼠标对应nrf52840gmouse_nrf52840, 
dongle对应nrf52840dongle_nrf52840，
其它默认。

★非常重要：Extra CMake Build Option可参考上面链接，填写-DCMAKE_BUILD_TYPE=ZReleaseB0，这样才可切换到，可以使用在线更新固件的release版本。

6）工程文件编译完后，在nrf_desktop下有对应的目录（如：build_nrf52840gmouse_nrf52840\zephyr），找到dfu_application.zip,覆盖对应dongle或mouse_dfu_release/configurator_cli下对应文件即可。

7）固件更新工具使用dongle_dfu_release和mouse_dfu_release下的批处理文件。
