# 📌 Box Radius Progress
Uma include para Pawn que permite criar barras de progresso copm borda usando `TextDraws`. Ideal para sistemas de hud, ações de tempo ou feedback visual para jogadores.

## Instalação

1. Baixe a versão mais recente do include `box_radius.inc`.
2. Coloque o arquivo na pasta `include/` do seu servidor.
3. Inclua no seu gamemode ou filterscript:

```pawn
#include <box_radius>
```
4. Instale [YSF](https://github.com/IllidanS4/YSF).

---

## ⚙️ Nativas
```pawn
native CreatePlayerBoxRadius(playerid, Float:pos_x, Float:pos_y, color = 0x1E90FFFF, bgcolor = 0x1C1C1CFF, Float:size = 5.0);
native UpdatePlayerBoxRadiusProgress(playerid, id, Float:value);
native DestroyPlayerBoxRadiusProgress(playerid, id);
native DestroyPlayerBoxRadiusAll(playerid);
```
> [!IMPORTANT]
> - `color`: Cor do progresso.
> - `bgcolor`: Cor de fundo.
> - `size`: Tamanho base da barra.
> - `value`: O valor de progresso vai de 0 a 100.


## 📝 Exemplo

```pawn
CMD:progresso(playerid, const params[])
{
    new id = CreatePlayerBoxRadius(playerid, 320.0, 150.0);
    UpdatePlayerBoxRadiusProgress(playerid, id, 50.0); // 50%
    return 1;
}
```

## 📷 Video

https://github.com/user-attachments/assets/26d3ed26-a75f-4dba-983d-481b4e50b5b3

## 📝 Créditos
- Ortex - Criador do codigo.

## 🌐 Outros idiomas
* [Português](https://github.com/dev-ortex/box-radius-progress/blob/main/READMPT.md)
* [Inglês](https://github.com/dev-ortex/box-radius-progress/blob/main/README.md)