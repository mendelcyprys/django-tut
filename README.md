### Django tutorial

Following the Django tutorial from the official documentation [here](https://docs.djangoproject.com/en/5.0/intro/tutorial01/).

#### First 8 lessons complete

After this they move to further/advanced topics, I will try to modify the project instead. The plan is to add bootstrap for some styling, and htmx - for example to show the poll results, so that a full page reload isn't triggered.

This is mainly because I want to learn some htmx and you need some server side system set up to use it (to return the html components), so I figured that this is a good place.
Both can be added simply for development via a CDN.

This will also give the opportunity to learn more about the Django templating language, hopefully.

#### Including the CSRF token

For `hx-post` you need to supply the CSRF token, one way of doing this is adding the attribute `hx-headers='{"X-CSRFToken": "{{ csrf_token }}"}'` to the body tag in the html template.

For a simple way to limit a view to a certain http request method, see [here](https://docs.djangoproject.com/en/5.0/topics/http/decorators/). 
