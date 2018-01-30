# vuejs-toggle-switch
Toggle switch for vue.js 2+

[Live demo](http://softwarefun.no/#/toggleswitch)

Install:
```bash
npm install vuejs-toggle-switch --save
```

Import: (in your main.js)
```javascript
import ToggleSwitch from 'vuejs-toggle-switch'
Vue.use(ToggleSwitch)
```

Use: (in your local .vue file/component, html section)
```xml

      <toggle-switch
        preSelected="Map"
        :labels="{map: 'Map', transit: 'Transit', satellite: 'Satellite'}"
        :width="380"
        :height="24"
        :padding="2"/>
```

### Properties

| Name      | Type              | Default     | Description                        |
| ---       | ---               | ---         | ---                                |
| width     | Number           | 100       | Width of item|
| height      | Number           | 34       | Height |
| padding     | Number           | 7       | padding |
| backgroundColor      | String           | white       | background color |
| color     | String           | black       | text color|
| borderColor      | String  | #007aff | border color |
| selectedColor     | String           | white     | text color selected item |
| selectedBackgroundColor      | String           | #007aff       | selected item background color |
| fontFamily     | String           | Lucida Grande       | font of item text |
| fontSize      | Number           | 14     | text size |
| disabled     | Boolean           | false       | disable switch |
| preSelected     | String           | unknown       | set pre selected item |
| labels     | [String, Object]           | n/A       | disable switch |

### Events

| Name   | Description              |
| ---    | ---                      |
| change | Triggered whenever state of the component/switch changes, @change="vmValueItem = $event.value" |
