# Home Assistant

Personal collection of Home Assistant blueprints, automations, and integrations.

---

## Blueprints

### Climate

| Blueprint | Description |
|---|---|
| [Window Open – Climate Off (Restore Mode)](blueprints/automation/window-open-climate-restore-mode.yaml) | Turns off a climate device when a window opens. When the window closes, choose to **restore the previous state** or **switch to HVAC mode `auto`**. Supports optional delay times and custom actions. |
| [Window Open – Climate Off (Advanced)](blueprints/automation/window-open-climate-advanced.yaml) | Extended version: choose to restore the previous state or **set a specific HVAC mode**. When not using `auto`, also control the temperature — restore the saved value, set a fixed target, or leave it unchanged. |
| [Heating Control – Away & Coming Home](blueprints/automation/heizung_presence.yaml) | Controls all heating devices based on `zone.home`. Switches all heaters to the **Away preset** when nobody is home, and to the **Home preset** when someone returns. Supports optional window sensors per heater — open windows are skipped. |

---

## Installation

Copy the desired YAML file into your Home Assistant config directory under the matching path, e.g.:

```
config/
└── blueprints/
    └── automation/
        └── window-open-climate-restore-mode.yaml
```

Then reload blueprints in Home Assistant: **Settings → Automations → Blueprints → Reload**.
