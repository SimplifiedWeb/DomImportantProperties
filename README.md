<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

<body>
  <h1>Zoom it and Read it Carefully I explained this in detail, You'll understand that correctly and Use it on your own</h1>
  <h4> understand the concepts and try it for one time</h4>
  <div class="section">
    <h2>offset (X and Y)</h2>
    <p>so when you use the offset property in any of the element that give the distance value from that particular target element. for example, a box have width of 300px and height of 300px and you target this box by, using some event, like click, mousemove etc and try to print the offset of that event.offsetX or Y, then you see that the offset give you the value from the target point. if you click on the center of the box, the distance from top and left to the point you target, the value you get. so remember that this property provides you the distance values from the specified point within the target element.</p>
    <h5>In hindi means, jab box ke kisi bhi jagah par click karenge then wo jagah se lekar edges tak ki value miligei
uss particualar box mai, agr beech mai click karenge to center se top tak ke value and left tak ki vlaue milegi,
ye sirf wo particular box tak hee rahaige

so remember that this property provides you the distance values from the specified point withing the target element.</h5>
  </div>

  <div class="section">
    <h2>client (X and Y)</h2>
    <p>so this property basically gives you the entire webpage viewport which is visible to you screen, That is the only difference between offset and client. client give you the full widht and height of the visible part of your screen. so when you click on the right side it give you the distance from the left to right like if you click on the right side of the viewport then it give you like 1230px for example. and one you click on the left side fo the viewport then it give you like 10px for example. so basically we it gives the value of the visible portion of the screen. if we shrink the window make it smaller then these client property gonna reflect and change accordingly. so remeber that client used for entire viewport section. and offset used for target element. it calculate only the distance values from that particular target container.</p>

    <h5>In Hindi,
Jitna apne ko screen pe show hota hai utni pure ko ye target karta hai so apun agar ismai koi event lagyenge or try
karenge log karne ka to smjhe ga, jitna mai mouse right mai leke jonga utni uski value badegi, it doesn't matter
ki wo jagah pe kitne element hai, maine bola jitna dikhrah hai white screen wo sab kuch consider karega.
so ye pure viewport ke liye hai, agge leke jayenge to increase value dega left kee taraf leke jayenge to decrease
value dega same up and down ke liye bhi hai. jitna neeche ayenge utna increase hogi jitna uper jayenge utna decrase hogi.</h5>
  </div>

  <div class="section">
    <h2>offsetWidth and offsetHeight</h2>
    <p>This is simple we can say that it give height and width of the target container. that's all if your container width is 500px then offsetWidth gives you 500px same for offsetHeight it gives you height of the container.</p>
  </div>

  <div class="section">
    <h2>scroll (X and Y)</h2>
    <p>basically in most commonly cases we use this for scrolling behaviour like we use window.scrollY or X. scrollTop we basically use on elements. like we can use the scrollTop in container to see how far we will from the top. so just keep in mind that, the scrollX and y property basically use for entire webpage to see the scrolling values. or some other stuff, basically used in parallex scrolling, or scrolling behaviours etc And the scrollTop and scrollLeft give us the values of the target element how much we scrolled. so we use different kind of stuff on the target reaching point of the scroll values, doing some kind of animation etc in both the cases. pageYoffset is same as scrollY. And remember one this if you see pageYoffset or pageXoffset it is same as the scrollY and scrollX doesn't get confused.</p>
  </div>

  <div class="section">
    <h2>clientWidth and clientHeight</h2>
    <p>so basically it is 90% similar like offsetWidth and height, the only difference is, it only give the content area of the element and padding, doesn't add the border, scrollbar. same for the clientHeight. so in offsetWidth and height it gives everything content area of the element, padding, border, scrollBar width if present. overall the functionality are same.</p>
  </div>

  <div class="section">
    <h2>innerHeight and innerWidth</h2>
    <p>Basically a viewPort height, if we shrink its values get changed. it gives us the height and the widht of the visible portion of our screen in webpage.</p>
  </div>

  <div class="section">
    <h2>getBoundingClientReact()</h2>
    <p>so somewhere i see getBoundingReact so basically they both are same. so always remember we use this for moving an elment from one place to another, for finding distance of an element within its parent container, and resizing its width and height we can control everything using this property. so we have to target an element and use this all properties and make it animated. like increasing the heigh and width of the element. just do that whatever variable you assign the values of getBounding property take that variable and use the .height .width .left .right and store that in box.style.width height left or right whatever property you are working on so you can get the scrolling effects etc whatever requirement you have. Hope this explanations helps you. </p>
  </div>

  <div class="section">
    <h2>Usage Example</h2>
    <p>Here's an example of using getBoundingClientRect() to trigger an animation:</p>
    <pre><code>
      const secondSectionMove = secondSection.getBoundingClientRect();
      console.log(secondSectionMove.top);
      if (secondSectionMove.top < window.innerHeight / 2) {
        box.style.transform = "translateX(0)";
      }
    </code></pre>

        <p>now you see in this example, i target the seconsection contianer that has the widht of 100vw and height of 100vh

and what I'm doing here, see the if statement, what it means, innerHeight is greater than secondSectionMove.top
then run that inside thing.

innerHeight gives us height of the visible portion of the screen.
and i use the scroll event to my function and by default if i can't scroll the value should be 0 right,
so when i scroll down the value gonna increase step by step so when we incounter our section we see the transition
effect.

getboudindClienReat watching the scroll that user performing how much is the distance from the top to the section2 where i use the property. the more we come close to that section the less value of 
top we get.

in Hindi, secondSectionMove.top ka mtlb ye hai ki bhai ye jo container hai mera section2 jismai maine property lagaya hai wo ye dekh rha hai ki kitna fasla hai uper se mere container thk getBoudingClientREact ye dekh raha, jaise jaise mai scroll karke uske nazdeek araha ho waise waise uski top ki vale come horahi hai, understand. and innerHeight to malum hai apko. Now calculate you will understand better

we can do some more calculation like multiply it or divide it by 2 at innerHeight to get the effect at the 
half of the screen when we scroll down. 


you can practice and try it on you own you can understand that better. 
</p>
  </div>
</body>
</html>
