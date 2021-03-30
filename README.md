# liken-android-public
The "presentation" repository of Liken by KaosClub

[App on Google Play](https://play.google.com/store/apps/details?id=br.com.kaosclub.liken)

Liken is a way to recommend (user to user) and get recommendations about movies and tv series. Users can create a recommendation of a content based another content. For example: I recommend "Zodiac" for that users that liked "Memories of Murder".

# Creators of the Android version
## Alan Kenji: creator and UX/UI designer
- [linkedin](https://www.linkedin.com/in/alan-yamasaki/)
- [behance](https://www.behance.net/alankenjiy)
- email: alankenjiy@gmail.com

## Luis Felipe: developer
- [linkedin](https://www.linkedin.com/in/luis-felipe-de-almeida-da-silva-42aa6016b/)
- email: luisfelipeas5@gmail.com
- github: [luisfelipeas5](https://github.com/luisfelipeas5)

# Preview
Short video and picture of the system

# Design
Some text that Alan want to put

# Main features
- Recommendation: shows two contents liken, a text justifying why user created this recommendation and possible comments done by others users;
- Content detail: has poster, synopsis, the MovieDb rating, access to watch trailer and recommendations created for that;
- Home: list the main movies and tv contents now a days;
- Search: show contents and users based in a query;
- Trending: in the future, this tab must show the recommendations based in relevance, but because some limitations, this tab is showing the last recommendations created;
- Watchlist: this tab show the contents that user added on Watchlist, Watched list and Favorite list;
- Profile: user can see favorite list and some personal data of some user in the system;

# System Archtecture
![alt text](https://github.com/luisfelipeas5/liken-android-public/blob/main/system_arch.jpg?raw=true)
- Mobile app: connect all parts in a beatiful UI;
- [The MovieDb Api](https://developers.themoviedb.org/3/getting-started/introduction): provide the content database;
- [Firestore of Firebase](https://firebase.google.com/docs/firestore): store recommendations, user data, watchlist, upvotes and comments;
- [Authentication with Firebase, Facebook and Twitter](https://firebase.google.com/docs/auth/android/start): authenticate users for create recommendations and create a watchlist.

# Android Archtecture
Built using:
- Model-View-ViewModel (MVVM) archtecture (using [LiveData](https://developer.android.com/topic/libraries/architecture/livedata) library for View <- ViewModel);
- Dynamic fueature modules/multi-modules. Prepared for on-demand features or instant-apps, but not ready.

# Libraries, plugins and techniques
- Navigation: [Navigation Archetecture Component](https://developer.android.com/guide/navigation)
- Dependency injection: [Insert Koin](https://insert-koin.io/)
- Animations: [Lottie](https://airbnb.io/lottie/#/), [Property Animation](https://developer.android.com/guide/topics/graphics/prop-animation) and "Animation Utils"
- Async operations: [Coroutines](https://developer.android.com/kotlin/coroutines)
- Local database: [Room](https://developer.android.com/training/data-storage/room)
- Push notifictions: [One signal](https://onesignal.com/)
- HTTP requests: [Retrofit](https://square.github.io/retrofit/)

# Curiosities
- the app born with Model-View-Presenter (MVP) archtecture and multiple activities based, using explicit intents by full name of the activity
