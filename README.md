The module itself:
```json
"custom/battery": {
    "format": "{icon} {}%",
    "format-icons": {
        "fully-charged": "󰁹",
        "pending-charge": "󰂄",
        "charging": "󰂄",
        "pending-discharge": "󰂑",
        "discharging": ["󰂎", "󰁺", "󰁻", "󰁼", "󰁽", "󰁾", "󰁿", "󰂀", "󰂁", "󰂂", "󰁹"]
    },
    "exec": "stdbuf -o L $HOME/.config/waybar/battery.sh BAT1 2> /dev/null",
    "return-type": "json"
}
