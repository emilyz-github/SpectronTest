# SpectronTest
Test Electron using Spectron

# Requirements
Test Electron with following scenarios:
- a button
- fill in a value to a input field
- has two pages, clicking on button on the first page, will open the second page. Verify the second page.

# Pre-requisite
- Javascript
- NodeJS
- Electron
- Spectron

# Sample
## WindowCount
app.client.waitUntilWindowLoaded()

		.getWindowCount().then(count => {
		
			t.is(count, 1);
			
		})
		
## Get Value from an input field
app.client.getValue('#form input[name=first]'))
## Click a button
app.client.click('#form input[name=add]');
