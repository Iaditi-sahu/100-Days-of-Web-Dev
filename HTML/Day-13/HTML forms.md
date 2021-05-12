# HTML Forms
** HTML form elements let you collect input from your website’s visitors. Mailing lists, contact forms, and blog post comments.Forms are the “money pages.” They’re how e-commerce sites sell their products, how SaaS companies collect payment for their service, and how non-profit groups raise money online.
** There are two aspects of a functional HTML form: the frontend user interface and the backend server.
** The action attribute defines the URL that processes the form. It’s where the input collected by the form is sent when the user clicks the Submit button. This is typically a special URL defined by your web server that knows how to process the data. Common backend technologies for processing forms include Node.js, PHP, and Ruby on Rails, but again, we’ll be focusing on the frontend in this chapter.
** The method attribute can be either post or get, both of which define how the form is submitted to the backend server. 
** thumb is to use post when you’re changing data on the server, reserving get for when you’re only getting data.
** By leaving the action attribute blank, we’re telling the form to submit to the same URL. Combined with the get method, this will let us inspect the contents of the form.