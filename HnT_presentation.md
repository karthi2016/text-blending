---- .aligncenter .bg-black
@unsplash(Szh_h2Avh5w) .dark

.text-data **Bricolage Zounderkite**
@h4 blending authors to make idiot soup with neural networks


@footer @div .wrap @div .span
 @button(href="https://github.com/thoppe/text-blending") .alignleft .ghost
   ::github:: Project repo
 @button(href="https://twitter.com/metasemantic") .ghost .alignright
   ::twitter:: @metasemantic 

---- .bg-white 

@h3 .size-80 .wrap
  .alignleft I like building deep learning architectures, <br>
  .alignright to explore what it means to be an algorithm, <br>
  .alignleft and define a bot by what it has experienced.
<br> <br> <br> 
@h3 .size-80 .wrap
  .alignleft If we can teach machines to talk like us, <br>
  .alignright we can use them to create a new medium, <br>
  .alignleft that remixes the past in a new way. 

---- .bg-black

.wrap 
 # .text-data Building an author bot
 
 ###
  + Download a large corpus of text 
  + Train a two-layer LSTM RNN over random sentences
  + Use Tensorflow (with Keras) to quickly prototype
  + Fix the top layer and train each author over the bottom layer
  
  _now bots share a common vocabulary!_

---- .bg-black 
@unsplash(MzIiekUr6m8) 

.size-60 .bg-trans-dark .alignleft
  @h4 .text-landing **Lovecraft bot** 
  .text-intro ... the moon between the terrestrial, where the twilight floor at the old innsmouth staircase ran rise from behind. No one could not absent to all the thing of publicly suggestion. above my frightful more I suspected that the

  @line
    
  @h4 .text-landing **Hemingway bot**
  .text-intro ...the moon will clear the cold. I was like a brown mother. Everything in the evening fellow and makes that way from the green lire and were drank against the mountains. The sun was on the branch contempt.

---- .bg-black

.wrap 
 # .text-data Blending bots
 
 ###
  + Sample a character from each bot
  + Choose which bot gets to speak with probability:
  + $f_1=\alpha; f_2 = (1-\alpha)$
  + Restart word if it doesn't exist in author vocabulary
  + Parallel sample and choose best paragraph

---- .size-70

@h3 .text-landing Shakespeare <br> to Lovecraft
.text-context .text-intro

  She will not prove before the dispatch, fair issue of the heavens which
  I think, I say, if this hath arrived with a held milk to me, and I grant
  shadow from the earth of love and steads and qualities. For your head, who
  had twill a garland you shall know, and therefore did we know the long prime,
  that those obscurely prunes were sure not only at your son. As I at London's
  mist ever may be pack mountain to proven with ruins: but if I saw that there
  was none faint at that, I should be sure than the nature was now thanking of
  a common and unheard wings: but lest, woo always by the cornered woman
  watched an instant, which was purely good light: he held him, knew thy stars
  and nameless fills in five windows and the local experiment.

---- .size-70

 @h3 .text-landing Tolstoy to Joyce
 .text-intro .text-context

  They are lying, but bonded out in danger as lovely? "I hope they are to say
  anywhere, I'm a new money. I am for I'd invent it a folk are not leaving
  to marry?" asked then at all. "Don't know what I have in his mind". Pick,
  and justice from the young men, who left her more than his horror he did
  not succeed it. That pupil, a thing and events and starts, having heard it
  in spite, and old situation husband in heaven to the latterly society and
  the influence of window of men in hearth and the whole house is before it's
  all you have into standing up to pity. do you know that about the dark?
  Perished the candles and the fair waves had a gentle interest.

---- .bg-black

.wrap 
 # .text-data Improvements?
 
 ###
  + Use word-based RNN
  + Enforce grammar as we do with words?
  + Use authors with _very_ distinct style (Chuck Tingle?)
  + Meld human and bot authorship.

---- .bg-black .slide-bottom
@unsplash(refAFfV35Cw)

# .text-landing Thanks, you!

### [https://github.com/thoppe/text-blending](https://github.com/thoppe/text-blending)
### [@metasemantic](https://twitter.com/metasemantic")