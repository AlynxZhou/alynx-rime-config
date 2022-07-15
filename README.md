alynx-rime-config
=================

Alynx's RIME configuration files.
---------------------------------

# Usage

First backup your old ibus-rime config.

This uses Luna Pinyin and Aurora Pinyin, so you need to install `rime-luna-pinyin` from official repo and `rime-aurora-pinyin` from AUR. It also depends on `rime-emoji` for emoji (only use it's opencc dict, I have a custom patch) and `rime-pinyin-zhwiki` for extended dictionary. If you are Arch Linux users, just run those commands to install them all (thanks to felixonmars).

```
# pacman -S librime ibus-rime rime-luna-pinyin rime-emoji rime-pinyin-zhwiki
$ paru rime-aurora-pinyin
```

If you are not Arch Linux users, I assume you know how to get those config for RIME, because I don't know.

Then clone this repo.

```
$ git clone https://github.com/AlynxZhou/alynx-rime-config.git ~/.config/ibus/rime
```

About emoji related stories, see <https://github.com/rime/rime-emoji/blob/master/README.md#%E8%87%AA%E5%8A%A9%E5%AE%89%E8%A3%9D>, <https://github.com/rime/rime-emoji/issues/16> and <https://github.com/hosxy/rime-aurora-pinyin/issues/13>.

Then trigger RIME's deploy. `ibus restart` or `ibus-daemon -rdx` or click deploy button (recommanded).

For detailed features in Chinese please go to my blog article: <https://sh.alynx.one/posts/My-RIME/>.

