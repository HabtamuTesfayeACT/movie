# movie
## Introduction

Welcome to my web! I am excited to have you here and hope you enjoy your browsing experience. In this README blog, we will provide you with information on what you can expect to find on our web, how to navigate it, and some of the key features that we offer.

## **Getting Started**

To start browsing our my, simply type [https://habtamutesfayeact.github.io/movie/index.html](https://habtamutesfayeact.github.io/movie/index.html) and press enter. Once you arrive on our homepage, you will be greeted with a clean, simple design that is easy to navigate. Our homepage features a menu bar at the top, which provides links to all of the different sections of the web

## Navigation

To navigate our web, simply click on any of the links in the menu bar at the top of the page. You can also use the search bar on our homepage to search for specific keywords or phrases related to the content you are interested in. Once you arrive on a new page, you will find that our web is designed to be easy to read, with clear headings and subheadings that make it simple to find the information you need.

## How does it work

T**he First javascript file named detail.js working with index.html**

I used JavaScript code that fetches data from the IMDb API to display the most popular movies and TV shows. It also allows users to search for movies using the IMDb search API. The code uses event listeners to shrink the navigation bar and to handle clicks on movie and TV show items.

The code begins with an event listener that calls the **`navbarShrink()`** function to shrink the navigation bar when the page is loaded or scrolled. The function gets the **`#mainNav`**
 element and adds or removes the **`navbar-shrink`** class depending on the value of the **`scrollY`**
 property.

The next part of the code defines the **`fetchMovies()`** function that fetches data from the IMDb API using the **`apiKey`** and **`baseURL`** constants. It returns a promise that resolves to an array of movie items. 

The **`fetchMovies()`** function is called when the page is loaded, and the resulting movies are displayed using the **`Movie()`** function. The **`Movie()`** function creates a new **`div`** element for each movie item, adds an **`img`** element with the **`src`** set to the **`poster_path`** property, and a **`p`** element with the movie title. It also adds a **`click`** event listener to the **`div`** element that redirects the user to the **`detail.html`** page with the **`movieId`** parameter set to the **`id`** property of the movie.

The code also defines a **`searhMovies()`** function that gets the value of the search input, fetches data from the IMDb search API using the **`searchUrl`** constant and the search query, and displays the resulting movies using the **`MovieResult()`** function. The **`MovieResult()`** function is similar to the **`Movie()`** function, but it uses the **`image`** and **`title`** properties of the search results instead of the movie items. If no movies are found, it displays a "No movies found" message.

Finally, the code defines a **`fetchSeries()`** function that fetches data from the IMDb API for the most popular TV shows, and displays them using the **`seriesMoveis()`** function. The **`seriesMoveis()`** function is similar to the **`Movie()`** function, but it displays TV show items instead of movies. It also adds a **`click`** event listener to the **`div`** element that redirects the user to the **`seriesDetail.html`** page with the **`seriesId`** parameter set to the **`id`** property of the TV show.

T**he second javascript file named detail.js working with detail.html**

Overall, this code provides a simple interface for browsing and viewing details of movies and TV shows, and related content based on the **`movieId`**, **`seriesId`**, and **`val`** parameters.

The **`Movie()`** function is used to create a new **`div`** element for each related movie or TV show, add an **`img`** element with the **`src`** set to the **`poster_path`** property, and a **`p`** element with the movie or TV show title. It also adds a **`click`** event listener to the **`div`** element that redirects the user to the **`detail.html`** or **`seriesDetail.html`** page with the corresponding **`movieId`** or **`seriesId`** parameter.

If **`val`** is **`0`**, it fetches the details for the TV show with the given **`seriesId`** using the IMDb API and displays the TV show poster, title, overview, release date, type, and stars using the **`detailseries`** URL and the **`fetch()`** method. It also fetches the related TV shows using the **`relatedSeriesUrl`** URL and displays them using the **`fetchRelatedseries()`** and **`Movie()`** functions.

The code first checks the value of the **`val`** parameter to determine whether to display movie or TV show details. If **`val`** is **`1`**, it fetches the details for the movie with the given **`movieId`** using the IMDb API and displays the movie poster, title, overview, and release date using the **`detailMovie`** URL and the **`fetch()`** method. It also fetches the casts and related movies using the same URL and displays them using the **`fetchcasts()`** and **`fetchRelatedMovies()`** functions, respectively. The **`castappend()`** and **`Movie()`** functions are used to append the cast and related movies to the HTML.

This is a JavaScript code that displays the details and related content for movies and TV shows based on the **`movieId`**, **`seriesId`**, and **`val`** parameters passed in the URL.

## Conclusion

We hope that this README blog has been helpful in providing you with an overview of our web and what you can expect to find here. If you have any questions or feedback, please don't hesitate to get in touch with us. We are always happy to hear from our visitors and are committed to providing you with the best browsing experience possible. Thanks for visiting our web, and we look forward to seeing you again soon!
