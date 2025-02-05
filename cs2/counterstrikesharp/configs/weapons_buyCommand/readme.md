### 功能说明

# 设置武器购买价格参见 weapons.json

```
   {
        "DefIndex": 16,
        "Name": "M4A1",
        "WeaponName": "weapon_m4a1",
        "Price": 3100,
        "Command": "M4A4",
        "Enable":true,
        "GunsMenu": true
    },
    {
        "DefIndex": 60,
        "Name": "M4A1-S",
        "WeaponName": "weapon_m4a1_silencer",
        "Price": 2900,
        "Command": "M4A1;m4a1s",
        "Enable":true,
        "GunsMenu": true
    }
```


# !zbuy 购买武器
-  如Enable为false 则不会出现在!guns菜单中,同时禁止 css_zbuy 指令购买
-  如GunsMenu为false 则不会出现在!guns菜单中,那么只能购买,如果用户选择被保存主武器则还原默认的m4a1,副武器为cz75a
-  command支持多个
-  比如 command: "fire;mov" !zbuy fire !zbuy mov
-  购买 zbuy mov
-  按键绑定购买燃烧瓶 控制台 `bind 键 css_zbuy fire`


# 限制手雷数量参数 注意下个回合生效(可以在地图参数中配置)
```css_hegrenade_limit 5```  
```css_molotov_limit 5```

  
# 该配置不在换图重读 需要重启服务器 可能需要2次.
