# NEXA Moonlight

Moonlight-common-c contém o código cliente central do GameStream compartilhado entre os clientes [Moonlight](https://moonlight-stream.org), incluindo [Moonlight PC](https://github.com/moonlight-stream/moonlight-qt), [Moonlight Android](https://github.com/moonlight-stream/moonlight-android), [Moonlight iOS](https://github.com/moonlight-stream/moonlight-ios) e [Moonlight Chrome](https://github.com/moonlight-stream/moonlight-chrome).

Se você está implementando seu próprio cliente de streaming de jogos Moonlight que pode usar uma biblioteca C, provavelmente deseja o código daqui.

## Nota para Desenvolvedores

Moonlight-common-c requer a _versão específica_ do ENet que é fornecida como um submódulo. Esta versão possui mudanças necessárias para compatibilidade com IPv6 e confiabilidade de retransmissão, entre outras coisas. Estas são mudanças na API/ABI que tornam o Moonlight-common-c incompatível com outras versões da biblioteca ENet. Tentar vincular em tempo de execução a outra biblioteca libenet causará o crash do seu cliente ao conectar com versões recentes do GeForce Experience.
