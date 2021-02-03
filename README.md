# Flickster
Flixster is an app that allows users to browse movies from the [The Movie Database API](http://docs.themoviedb.apiary.io/#).

📝 `NOTE - PASTE PART 2 SNIPPET HERE:` Paste the README template for part 2 of this assignment here at the top. This will show a history of your development process, which users stories you completed and how your app looked and functioned at each step.

---

## Flickster Part 1

### User Stories
`TODO://` In the **User Stories section below**, add an `x` in the `-[ ]` like this `- [x]` for any user story you complete. (🚫 Remove this paragraph after after checking off completed user stories)

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
<img src="https://github.com/henrylao/Flickster/blob/main/docs/portrait-editted.gif" width=250><br>
<img src="https://github.com/henrylao/Flickster/blob/main/docs/landscape-editted.gif" width=750><br>

### Notes
* Still experiencing difficulties when configuring the stars to be properly displayed need to do a little bit more research into the rating bar widget
* Still experiencing issues with images not being displayed despite async client properly fetching image urls requiring inclusion of <android:usesCleartextTraffic="true"> in the android MANIFEST.

### Open-source libraries used

- [Android Async HTTP](https://github.com/codepath/CPAsyncHttpClient) - Simple asynchronous HTTP requests with JSON parsing
- [Glide](https://github.com/bumptech/glide) - Image loading and caching library for Androids
