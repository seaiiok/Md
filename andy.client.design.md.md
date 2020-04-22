> Design for andy client

**依赖**
1. cobra [github.com/spf13/cobra]

**描述**
使用命令行界面的方式启动indy client。

**设计**
1.封装client客户端函数
2.通过命令交互.

**功能**

  **create**    Create invitation or seed.
  **exit**        Quit wallet.
  **get**         Get resources.
  **help**        Help about any command
  **init**        Init a new wallet.Input your name, wallet plugin path and gensis file.
  **message**     Send a message by connection id.
  **open**        Open your wallet.
  **quickstart**  Quick start - Register Did by Alice and active it.
  **register**    Register resources..
  **set**         Set resources.
  **version**     Show sdk version.
  **who**         Who am I?


<!--stackedit_data:
eyJoaXN0b3J5IjpbNDU4ODE5NDc3LDEyMTQwOTI2MDZdfQ==
-->