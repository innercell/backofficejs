#### [Go to the widgets folder](./js/components/page-widgets)

## List of widgets


### - [InfoBox](./js/components/page-widgets/info-box.js)

A basic info-box for displaying info. This component takes an options object, from props.

The options object needs 5 values.

```javascript
{
	color: 'bg-aqua' / 'bg-green' / 'bg-yellow', (To apply background color to the icon),
	icon: 'fa-envelope-o' / 'fa-flag-0' / 'fa-files-0', (Any font-awesome icon)
	subject:  'Can be a string or a number',
	stats: 'Can be a string or a number',
	content: 'Can be a string or a number'
}
```
##### Usage: 

```javascript

var infoBoxOptions = {
	color: 'bg-aqua',
	icon: 'fa-envelope-o',
	subject: 'Messages',
	stats: '1,410',
	content: '' 
};

<InfoBox options = {infoBoxOptions} />
```

![](../../screenshots/info-box.png)


### - [ProgressInfoBox](./js/components/page-widgets/progress-info-box.js)

An info-box for displaying info along with a progress bar. This component takes an options object, from props.

The options object needs 6 values.

```javascript
{
	color: 'bg-aqua' / 'bg-green' / 'bg-yellow', (To apply background color to the icon),
	icon: 'fa-bookmark-o' / 'fa-thumbs-o-up' / 'fa-calendar', (Any font-awesome icon)
	subject:  'Can be a string or a number',
	stats: 'Can be a string or a number',
	content: 'Can be a string or a number',
	progress: {
		percent: number, (For length of the progress bar, between 0-100) 
		description: 'Can be a string or number', (For the description in the progress bar)
		color: 'Any valid color in CSS3' (For the bar color)
	}
}
```
##### Usage: 

```javascript

var progressBoxOptions = {
	color: 'bg-green',
	icon: 'fa-thumbs-o-up',
	subject: 'Likes',
	stats: '41,410',
	content: '',
	progress: {
	    percent: 50,
	    description: '50% Increase in 30 Days',
	    color: 'white'
	} 
};

<ProgressInfoBox options = {progressBoxOptions} />
```

![](../../screenshots/progress-info-box.png)


### - [StatBox](./js/components/page-widgets/stat-box.js)

An box for displaying some basic info, highlighting numbers or stats. This component takes an options object, from props.

The options object needs 5 values, out of which 1 is optional

```javascript
{
	color: 'bg-aqua' / 'bg-green' / 'bg-red', (To apply background color to the icon),
	icon: 'fa-shopping-cart' / 'ion-stats-bars' / 'ion-person-add', (Any font-awesome icon)
	subject:  'Can be a string or a number',
	stats: 'Can be a string or a number',
	link: 'Link to go to for more information',	(Optional)
}
```
##### Usage: 

```javascript

var statBoxOptions = {
	color: 'bg-yellow',
	icon: 'ion-person-add',
	subject: 'User Registrations',
	stats: '44',
	link: '#' 
};

<StatBox options = {statBoxOptions} />
```

![](../../screenshots/stat-box.png)