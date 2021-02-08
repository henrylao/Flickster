## Flickster Part 2

### User Stories

#### REQUIRED (10pts)

- [x] (8pts) Expose details of movie (ratings using RatingBar, popularity, and synopsis) in a separate activity.
- [x] (2pts) Allow video posts to be played in full-screen using the YouTubePlayerView.

#### BONUS

- [ ] Implement a shared element transition when user clicks into the details of a movie (1 point).
- [x] Trailers for popular movies are played automatically when the movie is selected (1 point).
  - [x] When clicking on a popular movie (i.e. a movie voted for more than 5 stars) the video should be played immediately.
  - [x] Less popular videos rely on the detailed page should show an image preview that can initiate playing a YouTube video.
- [ ] Add a play icon overlay to popular movies to indicate that the movie can be played (1 point).
- [ ] Apply data binding for views to help remove boilerplate code. (1 point)
- [x] Add a rounded corners for the images using the Glide transformations. (1 point)

#### PERSONAL TWEAKS
- [ ] Implement gathering of all movies that are showing in theaters
- [ ] Implement a user login

### App Walkthough GIF

<img src="https://github.com/henrylao/Flickster/blob/main/docs/unit-2/detail-view-portrait-cropped.gif" width=250><br>

<img src="https://github.com/henrylao/Flickster/blob/main/docs/unit-2/detail-view-landscape-cropped.gif" width=750><br>

### Notes

* Researching and implementing the shared element transition proved to be challenging requiring refinement of understanding of the components involved
* Implementing the data binding for views was initially ambiguos and required further research before proceeding with implementation


## Flickster Part 1

### User Stories

#### REQUIRED (10pts)
- [x] (10pts) User can view a list of movies (title, poster image, and overview) currently playing in theaters from the Movie Database API.

#### BONUS
- [x] (2pts) Views should be responsive for both landscape/portrait mode.
   - [x] (1pt) In portrait mode, the poster image, title, and movie overview is shown.
   - [x] (1pt) In landscape mode, the rotated alternate layout should use the backdrop image instead and show the title and movie overview to the right of it.


- [ ] (2pts) Display a nice default [placeholder graphic](https://guides.codepath.org/android/Displaying-Images-with-the-Glide-Library#advanced-usage) for each image during loading

- [x] (2pts) Improved the user interface by experimenting with styling and coloring.
- [ ] (2pts) For popular movies (i.e. a movie voted for more than 5 stars), the full backdrop image is displayed. Otherwise, a poster image, the movie title, and overview is listed. Use Heterogenous RecyclerViews and use different ViewHolder layout files for popular movies and less popular ones.
- [ ] Implement deep scroll past the given 20 movies.
- [ ] Allow user to view details of the movie including ratings, genre and popularity in a seperate view.
- [ ] Create feature for viewing video trailers in both portrait or landscape mode.
- [ ] Create a feature for user account(basic info) and storing movies of interest
- [x] Implement star rating display feature on itemized view:
    - [x] Portrait mode
    - [ ] Landscape mode

### App Walkthough GIF
<img src="https://github.com/henrylao/Flickster/blob/main/docs/unit-1/portrait-editted.gif" width=250><br>
<img src="https://github.com/henrylao/Flickster/blob/main/docs/unit-1/landscape-editted.gif" width=750><br>

### Notes
* Still experiencing difficulties when configuring the stars to be properly displayed need to do a little bit more research into the rating bar widget
* Still experiencing issues with images not being displayed despite async client properly fetching image urls requiring inclusion of <android:usesCleartextTraffic="true"> in the android MANIFEST.

## Open-source libraries used
- [Android Async HTTP](https://github.com/codepath/CPAsyncHttpClient) - Simple asynchronous HTTP requests with JSON parsing
- [Glide](https://github.com/bumptech/glide) - Image loading and caching library for Android
