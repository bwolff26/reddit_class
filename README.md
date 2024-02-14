### Description

Nihonoku (fictional, per my quasi made up Japanese, roughly translating to 'Japanse paper'), a Japanese advertising company, has been noticing a growing trend of new manga (Japanese comic books) to be adapted into anime (Japanese cartoons). Wanting to see if the language of advertisements they used in the past for manga could be recycled with minimal changes to convert them into their anime equivelants, they outsouced to you, an otaku (a broad term that generally means somebody with way too much domain knowledge on anime and manga and the like) to first explore if the language used by otakus (the known consumer of such products) across both mediums is similar or not in the first place. Nihonoku is insistent on emulating the speach patterns of otaku, feeling that using their exact type of words is the key to maximizing profit. However, they would like to know how easily differentiable the two are, as the relative closeness of the two mediums would inversely call for a lesser allocation of assets to pay for a new ad in the future (working wtih an assumption that the language will be comprable for at least two years into the future), upon the anime adaption of a specific manga, as the original ad would already be closely fit to appeal to even its anime version. So, a special interest on precisely identifying animes is placed, as the higher it is would
indicate more of a need to prepare for changing the manga's script.

Secondardily, they are interested, time permitting, in the frequency of words that are neutral and popular to both, to strive to include marketing that revolves around themes that stand out - ideally being themes mutual to both of them.

Knowing that such otakus congregrate in mass in Reddit, you start to conduct a Natural Language Processing (NLP) centered exploration of the words used in both of their respective subreddits to see if it the two similar mediums can be differentiated. Thankfully, PRAW (Python Reddit API Wrapper) is available to expedite webscrabbing from them.

Be aware that the data was gathered in January 2024 - any findings may change due to shifting cultural references.

### Quoted Sources and Images

Data, originally pulled from:
-[manga](https://www.reddit.com/r/manga/)
-[anime](https://www.reddit.com/r/anime/)

-Naruto Art (manga, unsure what chapter that is from) via Marta on PinIntest.
-Naurto Art (anime) from Kortex of Deviant Art [Deviant Art](https://www.deviantart.com/kortrex/art/Naruto-Rasengan-479231732)
-Gintama (ep. 5) (warning: Ginpach-Sensei is not smoking a cigarette; he's eating a lollypop and smoke comes out "...because {he's} licking it so fast *proceeds to take it out and show Toshi, obviously shocked*.


### Conclusion

Initially, you sought to use the posts proper to differentiate between the two medias. However, the vast majority of mangas were blank, being posts of predominately pictures (and their analysis is beyond the scope of this project and in a way against our target). This resulted in a huge discrepency between anime and manga (being filled with at least their titles)'s word lengths. Furthermore, it was agreed upon that subsequent analysis would be invalid to properly evaluate language used when the datasets were so different. 

Ultimately, you were able to salvage the data by comparing their titles, that had very comporable lengths. You later built several models to identify manga and anime posts, with the 'best' model having an oveall accuracy of over 95% and a precision of over 94%. And, to emphasize: Despite titles being an average of 9 words each, we were still able to overwhelming predict one categoy from another. This realization beckons the company to be cautious, as even a small number of words is often indicativ of one category over another, especially when the estimated length of a commercial is likely comparable to that of a post. To potentially work around this quandry, it might be justfied in having a shorter commercial.

Additionally, you were able to start to identify several key words that were overwhelmingly (by a ratio of at least 2:1) in one of the two categories. However, more analysis is called for to properly suggest a proper list of neutral words to choose from that would not be tilting towards either direction.
