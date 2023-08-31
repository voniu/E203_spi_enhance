## E203_spi_enhance
蜂鸟 RISC-V 处理器 [E203](https://github.com/riscv-mcu/e203_hbirdv2) spi 外设的改进版本，原有功能未改动的基础上支持同时接收和发送。

### 如何使用
1. 使用 `apb_spi_master` 替换 E203 的 `apb_spi_master`（或者只替换 `spi_master_controller.v`）
2. 如 `driver` 内容所示修改 Hbird SDK
3. 使用驱动函数：[spi_sendAndReceive8](https://github.com/voniu/E203-SD-FatFs/blob/7b50524a639592113ee8487ea1e5b69786791e7c/src/sdcard.c#L139)
