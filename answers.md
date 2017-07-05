Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead.
PROTIP: use the inspector to learn the dimensions of the current profile image and use a placeholder image service such as Place Bear to get an image of the same size.

1) selecting the element that contains the profile image.
  document.querySelector('.profile-image')

2) change the src attirbute to point to a different picture
  var image = document.querySelector('.profile-image')
  image.src = "https://placebear.com/400/400"



Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing.
1) var skyImage = document.querySelector('img[title="Man Walking on Ice"]')
2) skyImage.src = "https://placebear.com/325/225"



Select the heading that says "Panda the Bear" and change it to your own name.
1) var title = document.querySelector('h1[class="highlight"]')
2) title.innerText = "Ronen Annason"

Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector)
1) var employ = document.querySelector('#employment')  --> select the object with id employment - which is the box that contains all the info
2) var info = employ.querySelector('.info-title')  --> select the title 'employment'
3) var icon = info.querySelector('.icon-suitcase')  --> select the suitcase icon
4)  info.innerHTML = icon.outerHTML + '  Unemployed' --> change the innerHTML of var info using concatination of icon.outerHTML and the string Unemployed. 

1) var employment = document.querySelector('#employment').querySelector('.info-title')
(not finished)

Change the colour of the body.
1)var body = document.querySelector('body')
2) body.style.background='red'


Change the colour used by the highlight class.

Change the font family of the h1 to 'monospace'.
1) var mono = document.querySelector('h1')
2) mono.style.fontFamily = 'monospace'


Find a way to select the round icons in the sidebar and then change their colour.

Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself".

Change the placeholder attribute of the message field to "state your business".

Give the name field a "value" attribute of "your nemesis".

Change the value attribute of the email field to "koalathebear@gmail.com".

Change the value of the submit button on the contact form to "En garde!".

We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute).

We should help Panda protect their privacy by clearing their personal details from the sidebar. You can use reset() to do this.
