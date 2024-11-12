---
runme:
  id: 01JC6Y9CJKMRCDDBRCS0ZWZDKC
  version: v3
---

## Output rendering

You can customize the way the cell output is rendered to be more human friendly, check it out.

#### Curl an image

You can visualize static and dynamic images inside your notebook.

Run the following curl command to render the beloved OpenTelemetry telescope logo:

```sh {"id":"01HTZB059ZFK301922YRJ9G5EW","interactive":"false,","mimeType":"image/svg+xml","name":"render-image-url"}
curl -s https://opentelemetry.io/img/logos/opentelemetry-horizontal-color.svg
```

#### Inspect JSON files

With [`antonmedv/fx`](https://github.com/antonmedv/fx) you can inspect JSON files interactively in Runme Notebooks.

Ensure you have **fx** installed (it requires [go](https://go.dev/)), run the following command:

```sh {"id":"01HTZB059ZFK301922YTAQ7XVY"}
go install github.com/antonmedv/fx@latest
```

#### Inspecting a curl response

Now you can explore any json file interactively, run the following command to explore the weather at Berlin 🍻

```sh {"background":"true","id":"01HTZB059ZFK301922YVFFN8R5","name":"interactive-json-fx","promptEnv":"no","terminalRows":"20"}
export FX_THEME="0"
curl -s "https://api.marquee.activecove.com/getWeather?lat=52&lon=10" | fx
```
