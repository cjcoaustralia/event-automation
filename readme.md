## Event Automation For Elements

### Basic Usage

1. Download the script file

2. Insert the script before `body` ends
	`<script src="main.js"></script>`
	or
	Insert our CDN
	`<script src="https://cdn.jsdelivr.net/gh/cjcoaustralia/event-automation/dist/main.js"></script>`

3. EventAutomation can be called without function call, it will be implemented automatically for all elements with `data-automation` attributes by the default.

4. Add `data-automation-start` and `data-automation-end` attribute to DOM elements for setting up the event period
For a specific timezone fill the `data-automation-country` with the country name and `data-automation-zone` with specific time zone by country. [Country and Timezones](http://worldtimeapi.org/timezones)
  

*Initial DOM without Timezone*

```html
<div
	data-automation
	data-automation-start="01-01-2023 05:35"
	data-automation-end="15-01-2023 23:59">
	Global Promotion till 16th Jan, 2023
</div>
```

*Initial DOM with Timezone*

```html
<div
	data-automation
	data-automation-start="01-01-2023 05:35"
	data-automation-end="10-01-2023 23:59"
	data-automation-country="australia"
	data-automation-zone="brisbane">
	Events in Brisbane till 10th Jan, 2023
</div>
```
