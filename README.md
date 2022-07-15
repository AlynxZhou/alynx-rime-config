alynx-rime-config
=================

Alynx's RIME configuration files.
---------------------------------

# Usage

First backup your old ibus-rime config.

This uses Luna Pinyin and Aurora Pinyin, so you need to install `rime-luna-pinyin` from official repo and `rime-aurora-pinyin` from AUR. It also depends on `rime-emoji` for emoji and `rime-pinyin-zhwiki` for extended dictionary. If you are Arch Linux users, just run those commands to install them all (thanks to felixonmars).

```
# pacman -S librime ibus-rime rime-luna-pinyin rime-emoji rime-pinyin-zhwiki
$ paru rime-aurora-pinyin
```

If you are not Arch Linux users, I assume you know how to get those config for RIME, because I don't know.

Then clone this repo.

```
$ git clone https://github.com/AlynxZhou/alynx-rime-config.git ~/.config/ibus/rime
```

If you are not using Arch Linux, you may need to add `emoji_suggestions.yaml`'s content to `luna_pinyin_simp.custom.yaml` manually and remove `__include: emoji_suggestion:/patch`. See <https://github.com/rime/rime-emoji/blob/master/README.md#%E8%87%AA%E5%8A%A9%E5%AE%89%E8%A3%9D> and <https://github.com/rime/rime-emoji/issues/16>.

Then trigger RIME's deploy. `ibus restart` or `ibus-daemon -rdx` or click deploy button (recommanded).

For detailed features in Chinese please go to my blog article: <https://sh.alynx.one/posts/My-RIME/>.

