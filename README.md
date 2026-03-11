# Home Assistant

Personal collection of Home Assistant blueprints, automations, and integrations.

---

## Blueprints

### Climate

| Blueprint | Description |
|---|---|
| [Window Open – Climate Off (Restore Mode)](blueprints/automation/window-open-climate-restore-mode.yaml) | Turns off a climate device when a window opens. When the window closes, you can choose to **restore the previous state** or **switch to HVAC mode `auto`**. Supports optional delay times and custom actions on open/close. |

---

## Installation

Copy the desired YAML file into your Home Assistant config directory under the matching path, e.g.:

```
config/
└── blueprints/
    └── automation/
        └── blaugrau90/
            └── window-open-climate-restore-mode.yaml
```

Then reload blueprints in Home Assistant: **Settings → Automations → Blueprints → Reload**.
