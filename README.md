# Balasclo, A forked project from Balatro ProperRussian by Nitablade.

Balasclo (**Bala**tro **S**implified **C**hinese **L**ocalization **O**verhaul) is a [Lovely](https://github.com/ethangreen-dev/lovely-injector)-based gathering of personal ideas of overhauling translated texts in the video game Balatro, containing various fixes, improvements, glossary unification, in conjunction with planned texture and font overwrite for a better game experience. 

This repository is a fork of [Nitablade's Balatro ProperRussian](https://github.com/Nitablade/Balatro_ProperRussian).

## 简要说明：
本项目当前适用于 Balatro 1.0.1f-FULL
请确保你已在 [**Lovely** 的发布页](https://github.com/ethangreen-dev/lovely-injector/releases)获取了最新的`version.dll`并存放于游戏的安装路径中（与游戏主程序`Balatro.exe`处于同一路径下）

## 为什么会有这个项目？

不知道是不是发行商被人坑了，Balatro 的官方翻译像是由五六个 CET6 勉强及格的半瓶晃荡攒出来的“工作室”做的。他们遇到生词可能会去百度查翻译，也从始至终没有一个统一的术语库，甚至未见得在翻译过程中打开游戏看过一两眼。

Balasclo 是一个个人色彩相对浓烈的本地化重置项目，大体包含对游戏原有本地化的修改和完善。大致包括：

- （占位）

此外，我也在为部分自己游玩的 Steamodded 模组制作简体中文本地化。这些模组的本地化使用了和 Balasclo 同样的术语库：

- [betmma/my_balatro_mods](https://github.com/ChromaPIE/betmma-mods-ZHCN-Locale) [原仓库](https://github.com/betmma/my_balatro_mods)
- [Firch/Bunco](https://github.com/ChromaPIE/Bunco-ZHCN-Locale) [原仓库](https://github.com/Firch/Bunco)
- [Aurelius7309/SixSuits](https://github.com/ChromaPIE/SixSuits-ZHCN-Locale) [原仓库](https://github.com/Aurelius7309/SixSuits)
- [notmario/MoreFluff](https://github.com/ChromaPIE/MoreFluff-ZHCN-Locale) [原仓库](https://github.com/notmario/MoreFluff)
- [itayfeder/Codex-Arcanum](https://github.com/ChromaPIE/Codex-Arcanum-ZHCN-Locale) [原仓库](https://github.com/itayfeder/Codex-Arcanum)
- []() [原仓库]()
- []() [原仓库]()

Balasclo 不会，也不计划加入未来可能的任何 Balatro 整合汉化项目。

---

В моде также заменён шрифт на доработанный **Mini Pixel 7**, не стремясь повторить оригинальный, но пиксельный, хорошо читабельный и вписывающийся в сеттинг. Альтернативный шрифт, копирующий англоязычный **m6x11plus** лежит в папке ```/extra```.

## Как установить (на Windows):
Подробный гайд на странице [Releases](https://github.com/Nitablade/Balatro_ProperRussian/releases)

Если не сложно, оставьте какую-нибудь реакцию и/или комментарий под этим постом для продвижения: (сначала присоединитесь к [офф. серверу Balatro](https://discord.gg/cbbuVAU9)): [https://discord.com/channels/1116389027176787968/1217140107962748949/1217140107962748949](https://discord.com/channels/1116389027176787968/1217140107962748949/1217140107962748949)

Спасибо.

## Как установить (на SteamDeck):
Установка происходит точно так же, как на Windows, отличаются только пути для распаковки файлов. А именно, .dll файл:
- Если игра установлена на SD-карте: ```primary/steamapps/common/Balatro```
- Если игра установлена во Внутренней памяти: ```Home/.steam/steam/steamapps/common/Balatro```  
Папка **Appdata** находится по пути: ```Home/.steam/steam/steamapps/compatdata/2379780/pfx/drive_c/users/steamuser/AppData/Roaming/Balatro```

## Как установить (на Mac):
- Пока неизвестно, за неимением Mac'а, если кто разобрался - напишите мне.

## Файловая структура мода:
- ```version.dll``` : Lovely-инжектор (необходим для применения написанных вручную патчей интерфейса, а также корректных параметров для шрифта)
- ```/mods/ProperRussian/lovely.toml``` : файл, содержащий все вручную написанные патчи, которые применяются поверх игры, не трогая код приложения и не влияя на получение достижений (к каждому патчу присутствует комментарий)
- ```/resources/textures/``` : папка содержит заменяемые игровые текстуры, которые хранятся в файлах ```BlindChips, Boosters, Jokers, ShopSignAnimations, Tarots и Vouchers``` (если хотите играть без них - просто удалите ненужные вам из папки ```/1x``` и ```/2x```)
- ```/resources/fonts/NotoSans-Bold.ttf``` : файл кастомного шрифта, заменяет основной шрифт, использующийся в оф. переводе (не влияет на английский шрифт, если вы захотите поиграть с ним), при желании можно заменить на любой другой шрифт, сохранив такое же название шрифта, а также заменив файл ```lovely.toml``` из папки ```/extra```
- ```/localization/ru.lua``` : файл перевода всех строк, использующихся в игре, в отличие от оф. релиза все строки отсортированы в том же порядке, что и в оригинальном ```en-us.lua```
- ```/extra``` : папка с необязательными к установке элементами, на данный момент содержит альтернативный шрифт и русифицированные текстуры для игральных карт

**Дополнительные опции / Как заменить отдельные элементы:**

Начиная с версии мода **1.0.5**, дополнительный шрифт и другие необязательные к установке опции перенесены в папку ```/extra```. Для их активации просто замените существующие файлы. На данный момент доступны следующие экстра-элементы:
- альтернативный шрифт (копирует стиль оригинального **m6x11plus**)
- русифицированные литеры для игральных карт (В - Валет, Д - Дама, К - Король, Т - Туз) для обычного и высококонтрастного режима

## Известные недочёты:
- В списке правил для испытания *Жестокость*, строка о Блайндах без наград отображается дважды
- Название Босс-блайнда *Лазурный колокольчик* не вмещается в HUD на экранах с разрешением 1080р и ниже

## Ниже немного скриншотов
![20240327181037_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/749be51a-b923-4833-909f-ae2f6607dafb)
![20240327181053_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/f42e2473-44a9-42c3-83ce-ac0c292c0ab0)
![20240327181107_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/ba86b08e-e3dc-4fa1-895a-784e33dd32e8)
![20240412044015_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/d0c9fda3-6549-436d-abbd-0533c801d2d5)
![20240327181211_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/29c19d05-456c-4ce9-94bc-d9c7133fcd76)
![20240327181234_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/d48b1cdf-ddbc-4f5f-b838-fc087bc46b6a)
![20240327181314_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/23ee7f4a-21c3-40d2-a853-b5438f2c7f91)

### Выразить благодарность автору локализации можно тут: [https://www.twitch.tv/Nitablade](https://www.twitch.tv/Nitablade)

Помимо Balatro, я занималась локализацией для таких игр как:
1) [**BEAM**](https://store.steampowered.com/app/1067430/Beam/)
2) [**Backpack Hero**](https://store.steampowered.com/app/1970580/Backpack_Hero/)
3) [**Мод Downfall**](https://steamcommunity.com/sharedfiles/filedetails/?id=1610056683&searchtext=Downfall) для Slay the Spire
4) [**Wildfrost**](https://store.steampowered.com/app/1811990/Wildfrost/) (Релиз перевода уже скоро)

Также можете присоединиться к моему [Discord-серверу](https://discord.gg/zFAGDn6QMs), чтобы следить за обновлениями локализаций.
