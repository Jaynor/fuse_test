# Fuse Test

## JS

> **Q1** I'd like to transform the elements of `myarr`  to `[11,12,13,14,15]`. Write code using the `map`.

     let myarr = [1,2,3,4,5];


## Fuse


>`hikes.js`

    var hikes = [
       {
        id: 0,
        name: "Tricky Trails",
        location: "Lakebed, Utah",
        distance: 10.4,
        rating: 4,
        comments: "This hike was nice .."
       },
       {
        id: 1,
        name: "Mondo Mountains",
        location: "Black Hills, South Dakota",
        distance: 20.86,
        rating: 3,
        comments: "Not the best..."
       },
       {
        id: 2,
        name: "Pesky Peaks",
        location: "Bergenhagen, Norway",
        distance: 8.2,
        rating: 5,
        comments: "Short but SO sweet!!"
       }
    ];

> `MainView.js`

    var Observable = ______("FuseJS/Observable");
    var myHikes = ______("hikes");

    var hike = Observable();

    module.exports = {
      hikes: myHikes,
      name: name,
      location: location,
      distance: distance,
      rating: rating,
      comments: comments,
    };

## Q2-Q3
> I want to store `hikes` from `hikes.js` into `myHikes` from`MainView.js`, what should I do ?


- **Q2** Fill in the blank
- **Q3** Add codes in `hikes.js`

> I want to capture the  --------

- **Q4** What's `Observable` ?

## Fuse Command Line
- **Q5** What's the the Fuse command to create a new app?
- **Q6** How to open a created app in Fuse?

##



> Previously, I had all JS codes in `MainView.ux` file like this.

    <App>
  	   <ClientPanel>
		<JavaScript>
			var Observable = ____("FuseJS/Observable");

			var hikes = [ ... ] ;
            </JavaScript>
       </ClientPanel>
    </App>

>After placing JS code into seperate `.js` files, my Fuse app failed to build. I realize I should have added this code chunk in a certain file.
**code**:`"hikes.js:Bundle"`

- ** Q7 ** Tell me in which file I should place this code chunk.
 - a.  `.gitignore`
 - b. `hikes.js`
 - c. `hikr.unoproj`
 - d. `MainView.ux`
 - e. `MainView.js`


`closing.ux`

    <App>
  	   <ClientPanel>
		<JavaScript>
			var Observable = ____("FuseJS/Observable");

			var hikes = [ ... ] ;
            </JavaScript>
        <StackPanel>
         <Text Value="{name}"></Text>
         <Text> Name: </Text>
         <TextBox Value ="{name}"></Text>
         <Text> Location: </Text>
         <TextBox Value ="{location}"></Text>
         <Text> Distance (km) : </Text>
         <TextBox Value ="{distance}" __(a)__ = "__(b)__"></TextBox
         <Text> Rating: </Text>
         <TextBox Value ="{rating}" __(c)__ = "__(d)__"></TextBox>
         <Text> Comments: </Text>
         <TextBox Value="{comments}" __(e)__="__(f)__"></TextBox>
         <Button Text="Back" __(g)__="{goBack}"></Button>
        </StackPanel>
      </ClientPanel>
    </App>


- **Q8** From the `closing.ux`, how many tags can be written like this example? **example**`<ExampleTag/>`
 - `<App>` :
 - `<ClientPanel>` :
 - `<JavaScript>` :
 - `<StackPanel>` :
 - `<Text>` :
 - `<TextBox>` :
 - `<Button>` :

> Match a code and an image.

- ** Q9** `<Text/>`
- ** Q10** `<TextBox/>`
- ** Q11** `<TextView/>`

> Fill in the blanks based on what we did.

- **Q12** (a)
- **Q13** (b)
- **Q14** (c)
- **Q15** (d)
- **Q16** (e)
- **Q17** (f)

> `<StackPanel/>`

- **Q18** Describe what `<StackPanel/>` does.




## JS
**Q19**
> I want have an array like this.
`var nameArr =["Tricky Trails","Mondo Mountains","Pesky Peaks"];`. Write codes to create `nameArr`, only using the array`hikes` in `hikes.js`. *(It's not allows to use hard-coded strings, which means if the name in `hikes` gets changes, your `nameArr` should be updated automatically.)*
