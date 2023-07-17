
<p align="center">
  <a href="" rel="noopener">
 <img width=150px height=50px src="https://cinesubz.co/wp-content/uploads/2022/10/cinesubz.co-Logo.jpg" alt="cinesub"></a>
</p>


<h2 align="center">Cinesubz Movie Downloader</h2>





## 📝 Table of Contents

- [About](#about)
- [Getting Started](#getting_started)
- [Usage](#usage)
- [Authors](#authors)

## 🧐 About <a name = "about"></a>

The unofficial Scrap <a href="https://cinesubz.co/" > [https://cinesubz.co/] </a>

## 🏁 Getting Started <a name = "getting_started"></a>

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Installing


```sh
yarn add @sl-code-lords/movie-dl
```

or

```sh
npm i @sl-code-lords/movie-dl
```

## 🎈 Usage <a name="usage"></a>

```ts
var { Cinesubz }  = require('@sl-code-lords/movie-dl')

```
## Get Movies/Twshows List By Search
```ts
var input = 'money heist' //movie or tvshow name
await Cinesubz.get_list.by_search(input) 
```


```ts
//result

{
  status: true,
  code_creator: { name: 'Thisal Sanujaya', github: '@sanuwaofficial' },
  results: [
    {
      title: 'Money Heist: Korea – Joint Economic Area (TV Series 2022) Complete Season 01',
      link: 'https://cinesubz.co/tvshows/money-heist-korea-joint-economic-area-tv-series-2022-complete-season-01/',
      type: 'tvshows'
    },
    {
      title: 'Money Heist (2021)  Sinhala Subtitle | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/tvshows/money-heist-2021-sinhala-sub/',
      type: 'tvshows'
    },
    {
      title: 'Hell or High Water (2016) Sinhala Subtitle',
      link: 'https://cinesubz.co/movies/hell-or-high-water-2016-sinhala-subtitle/',
      type: 'movies'
    },
    {
      title: 'Ambulance (2022) Sinhala Subtitle | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/ambulance-2022-sinhala-sub/',
      type: 'movies'
    },
    {
      title: 'Sapthamashree Thaskaraha (2014) Sinhala Subtitle | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/sapthamashree-thaskaraha-2014-sinhala-sub/',
      type: 'movies'
    },
    {
      title: 'Now You See Me (2013) Sinhala Subtitle | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/now-you-see-me-2013-sinhala-sub/',
      type: 'movies'
    }
  ]
}
```
## Get Recently added movies list

```ts
var page = 1 //page number
await Cinesubz.get_list.by_recent_movies(page)
```
```ts
//result

{
  status: true,
  code_creator: { name: 'Thisal Sanujaya', github: '@sanuwaofficial' },
  results: [
    {
      title: 'Bird Box Barcelona (2023) Sinhala Subtitles | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/bird-box-barcelona-2023-sinhala-subtitles/',
      type: 'movies'
    },
    {
      title: 'Crimson Peak (2015) Sinhala Subtitles | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/crimson-peak-2015-sinhala-subtitles/',
      type: 'movies'
    },
   18 more...
  ]
}

```
## Get Recently added tvshows list

```ts
var page = 1 //page number
await Cinesubz.get_list.by_recent_tvshows(page)
```
```ts
//result

{
  status: true,
  code_creator: { name: 'Thisal Sanujaya', github: '@sanuwaofficial' },
  results: [
    {
      title: 'Revenant (2023) S01 EP01-04',
      link: 'https://cinesubz.co/tvshows/revenant-2023-s01/',
      type: 'tvshows'
    },
    {
      title: 'Lies Hidden in My Garden (2023) S01 EP01-04',
      link: 'https://cinesubz.co/tvshows/lies-hidden-in-my-garden-2023-s01/',
      type: 'tvshows'
    },
    18 more...
  ]
}
```
## Get Movies/Tvshows List By Language
```ts
var lang = 'English' // Language ( ex : Sinhala , English , Tamil , Hindi , Kannada , France , Japanese , Telugu , Malayalam , Korean , Other )
var page = 1 //page number
await Cinesubz.get_list.by_language[lang](page)
```
```ts
//result

{
  status: true,
  code_creator: { name: 'Thisal Sanujaya', github: '@sanuwaofficial' },
  results: [
    {
      title: 'xXx: Return of Xander Cage (2017) Sinhala Subtitles | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/xxx-return-of-xander-cage-2017-sinhala-subtitles/',
      type: 'movies'
    },
    {
      title: 'xXx: State of the Union (2005) Sinhala Subtitles | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/xxx-state-of-the-union-2005-sinhala-subtitles/',
      type: 'movies'
    },
    18 more...
  ]
}
```

## Get Movies/Tvshows List By Genre
```ts
var genre = 'Action' // Genre ( ex : History , Thriller , Comedy ,  Horror , Adventure , Science_fiction , Mystery , Animation , Sport ,  Drama , Action , Crime , Romance , Fantasy , Family , War , Adult_only , Short )
var page = 1 //page number
await Cinesubz.get_list.by_genre[genre](page)
```
```ts
//result

{
  status: true,
  code_creator: { name: 'Thisal Sanujaya', github: '@sanuwaofficial' },
  results: [
     {
      title: 'xXx: Return of Xander Cage (2017) Sinhala Subtitles | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/xxx-return-of-xander-cage-2017-sinhala-subtitles/',
      type: 'movies'
    },
    {
      title: 'xXx: State of the Union (2005) Sinhala Subtitles | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/xxx-state-of-the-union-2005-sinhala-subtitles/',
      type: 'movies'
    },
    18 more...
  ]
}
```
## Get Movies/Tvshows List By Year
```ts
var year = '2023' // year
var page = 1 //page number
await Cinesubz.get_list.by_year(year,page)
```
```ts
//result

{
  status: true,
  code_creator: { name: 'Thisal Sanujaya', github: '@sanuwaofficial' },
  results: [
    {
      title: 'Mother’s Day (2023) Sinhala Subtitles | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/mothers-day-2023-sinhala-subtitles/',
      type: 'movies'
    },
    {
      title: 'Dream (2023) Sinhala Subtitles | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/dream-2023-sinhala-subtitles/',
      type: 'movies'
    },
    18 more...
  ]
}
```
## Get Movies/Tvshows List By Actor
```ts
var url = 'https://cinesubz.co/cast/dhanush/' // cast link
var page = 1 //page number
await Cinesubz.get_list.by_actor(url,page)
```
```ts
//result

{
  status: true,
  code_creator: { name: 'Thisal Sanujaya', github: '@sanuwaofficial' },
  results: [
    {
      title: 'Vaathi (2023) Sinhala Subtitles | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/vaathi-2023-sinhala-subtitles/',
      type: 'movies'
    },
    {
      title: 'Kodi (2016) Sinhala Subtitles | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/kodi-2016-sinhala-subtitles/',
      type: 'movies'
    },
    18 more...
  ]
}
```
## Get Movies/Tvshows List By Director
```ts
var url = 'https://cinesubz.co/director/s-s-rajamouli/' // director url
var page = 1 //page number
await Cinesubz.get_list.by_director(url,page)
```
```ts
//result

{
  status: true,
  code_creator: { name: 'Thisal Sanujaya', github: '@sanuwaofficial' },
  results: [
    {
      title: 'Chatrapathi (2005) Sinhala Subtitle | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/chatrapathi-2005-sinhala-sub/',
      type: 'movies'
    },
    {
      title: 'Original RRR (2022) Sinhala Subtitle | සිංහල උපසිරැසි සමඟ | TELUGU',
      link: 'https://cinesubz.co/movies/rrr-2022-sinhala-sub/',
      type: 'movies'
    },
    {
      title: 'Magadheera (2009) Sinhala Subtitle | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/magadheera-2009-sinhala-sub/',
      type: 'movies'
    },
    {
      title: 'Baahubali 2: The Conclusion (2017) Sinhala Subtitle | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/baahubali-2-the-conclusion-2017-sinhala-sub/',
      type: 'movies'
    },
    {
      title: 'Baahubali: The Beginning (2015) Sinhala Subtitles | සිංහල උපසිරැසි සමඟ',
      link: 'https://cinesubz.co/movies/baahubali-the-beginning-2015-sinhala-subtitles/',
      type: 'movies'
    }
  ]
}
```
## Get Movie Details and Download Links
```ts
var url = 'https://cinesubz.co/movies/original-k-g-f-chapter-2-2022-kannada-with-sinhala-sub/' // movie url
await Cinesubz.movie(url)
```
```ts
//result
{
  status: true,
  code_creator: { name: 'Thisal Sanujaya', github: '@sanuwaofficial' },
  result: {
    title: 'Original K.G.F: Chapter 2 (2022) KANNADA With Sinhala Sub',
    subtitle_author: 'ಕೆ.ಜಿ.ಎಫ್: Chapter 2',
    categories: [ 'Action', 'Drama', 'Kannada' ],
    release_date: 'Apr. 14, 2022',
    country: 'India',
    duration: '168 Min.',
    director: {
               name: 'Prashanth Neel',
               link: 'https://cinesubz.co/director/prashanth-neel/'
              },
    cast: [
           { name: 'Yash', link: 'https://cinesubz.co/cast/yash/' },
           { name: 'Sanjay Dutt', link: 'https://cinesubz.co/cast/sanjay-dutt/'},
           8 more...
          ],
    desc: 'The blood-soaked land of Kolar Gold Fields (KGF) has a new overlord now – Rocky, whose name strikes fear in the heart of his fo...',
    images: [
             'https://i0.wp.com/cinesubz.co/wp-content/uploads/2022/05/photo_2022-04-08_03-03-51.jpg?fit=226%2C300&ssl=1',
             'https://image.tmdb.org/t/p/original/nsV5Mfi9FAV4w8eDsdr7uqVswOk.jpg',
             7 more...
            ],
    dl_links: [
               {
                quality: 'HQ 1080p WEB-DL',
                size: '9 GB',
                link: 'https://d.cd38lk.workers.dev/1:/Movie2/2205/16/K.G.F%20Chapter%202%20(2022)%20Kannada%20(Org%20Vers)%C2%A0True%20Web-Dl%20-%201080P%20-%20Avc%20-%20Untouched%20-%20(Dd+5.1%20-%20640Kbps%20&%20Aac%202.0)%C2%A0-%209.5%20Gb%C2%A0-.mp4'
              },
              {
               quality: 'WEBDL SD 480p',
               size: '800 MB',
               link: 'https://d.cd38lk.workers.dev/1:/Movie2/2205/16/K.G.F%20Chapter%202%20(2022)%20Kannada%20(Orginal)%20TRUEWEB-DL-%5BCineSubz.com%5D-480P.mp4'
              },
              3 more...
              ]
           }
}

```
## Get Tvshow Details and episode Links
```ts
var url = 'https://cinesubz.co/tvshows/money-heist-2021-sinhala-sub/' // tvshow url
await Cinesubz.tvshow(url)
```
```ts
//result

{
  status: true,
  code_creator: { name: 'Thisal Sanujaya', github: '@sanuwaofficial' },
  result: {
    title: 'Money Heist (2021) Sinhala Subtitle | සිංහල උපසිරැසි සමඟ',
    categories: [ 'Crime', 'Drama' ],
    cast: [
           { name: 'Álvaro Morte', link: 'https://cinesubz.co/creator/alex-pina/' },
           { name: 'Úrsula Corberó', link: 'https://cinesubz.co/cast/alvaro-morte/' },
           8 more...
          ],
    links: [ 
            [
             { episode: '1 - 1',
               link: 'https://cinesubz.co/episodes/money-heist-1x1/'},
             {
              episode: '1 - 2',
              link: 'https://cinesubz.co/episodes/money-heist-1x2/' },
             11 more...
           ], 
           [
             { episode: '2 - 1',
               link: 'https://cinesubz.co/episodes/money-heist-2x1/'},
             { episode: '2 - 2',
               link: 'https://cinesubz.co/episodes/money-heist-2x2/' },
             7 more...
           ],
            3 more... 
          ]
  }
}
```
## Get Episode Details and download Links
```ts
var url = 'https://cinesubz.co/episodes/money-heist-1x2/' // episode url
await Cinesubz.episode(url)
```
```ts
//result

{
  title: 'Money Heist (2021) Sinhala Subtitle | සිංහල උපසිරැසි සමඟ: 1x2',
  desc: 'Knowing that the police won’t try to storm the building again after their first failed attempt, the robbers start to use the hostages to print money, to dig a tunnel for their escape, and to negotiate with the police. Raquel, who quit due to a verbal argument with Colonel Prieto after the failed rescue mission, meets a strange gentleman at a bar and gets suspicious. Because of Alison’s phone, the police is able to identify 2 of the robbers, Tokyo and Rio – and that’s not the only phone the robbers missed to collect.',
  release_date: 'May. 09, 2017',
  images: [
    'https://image.tmdb.org/t/p/original/e5sVue90Xd7kbTLrfbArexjpPEz.jpg',
    'https://image.tmdb.org/t/p/original/rVHvenlB4VcNeX7joIevfgZZBJR.jpg',
    5 more...
  ],
  links: [
    {
      quality: 'Direct Download WebRip 480P',
      size: '200 MB',
      link: 'https://d.cd013.workers.dev/1:/TV%20Series/Money.Heist/S01/CineSubz.com%20-%20Money.Heist.S01E02.SPANISH.480p.10bit.WEBRip.2CH.x265.HEVC-PSA.mp4'
    },
    {
      quality: 'Direct Download WebRip 720P',
      size: '400 MB',
      link: 'https://d.cd013.workers.dev/1:/TV%20Series/Money.Heist/S01/CineSubz.com%20-%20Money.Heist.S01E02.SPANISH.720p.10bit.WEBRip.2CH.x265.HEVC-PSA.mp4'
    }
  ]
}
```

## ✍️ Authors <a name = "authors"></a>

- [@sanuwaofficial](https://github.com/sanuwaofficial) - scraped project author

See also the list of [contributors](https://github.com/SL-CODE-LORDS/movie-dl/contributors) who participated in this project.
