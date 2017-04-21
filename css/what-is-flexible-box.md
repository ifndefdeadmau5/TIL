#Flexible boxes
https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Using_CSS_flexible_boxes#See_also

##Flex 의 용어들

flex-direction: row 일 때, 수평 축을 main axis 라 하고, 수직을 cross axis라 하며 이 때 cross start 가 위  쪽, cross end 가 아래 쪽이다.
flex-direction: column일 때는 이와 반대다.
flex box 내에서 각각 item들은 주축 방향에 따라 main size, cross size 로 불린다. 아래의 이미지 참고

###Flex container
플렉스 아이템을 감싸는 부모
###Flex item
플렉스 컨테이너 각각의 자식들, Flex container안에 생으로 텍스트를 넣을경우 익명의 Flex item으로 자동으로 감싸진다

###Axes

* The flex-direction property establishes the main axis.
    * main axis 를 설정한다
* The justify-content property defines how flex items are laid out along the main axis on the current line.
    * flex item 들이 main axis를 따라서 어떤 방법으로 놓여질지 결정한다.
* The align-items property defines the default for how flex items are laid out along the cross axis on the current line.
    * flex item들이 cross axis를 따라서 어떤 방법으로 놓여질지 결정한다.
* The align-self property defines how a single flex item is aligned on the cross axis, and overrides the default established by align-items.
    * flex item이 cross axis를 따라서 어떻게 정렬될지, align-items에 의해 정의된 기본값을 override 한다.

###Lines

Flex items can be laid out on either a single line or on several lines according to the flex-wrap property, which controls the direction of the cross axis and the direction in which new lines are stacked.

플렉스 아이템은 cross axis 방향과 새로운 줄이 생겨날 방향을 제어하는 flex-wrap 속성에 따라 한 줄 또는 여러 줄로 놓여질 수 있습니다.

###Dimensions

The flex items' agnostic equivalents of height and width are main size and cross size, which respectively follow the main axis and cross axis of the flex container.

* The min-height and min-width properties initial value is 0.
* The flex property shorthands the flex-grow, flex-shrink, and flex-basisproperties to establish the flexibility of the flex items.

https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Using_CSS_flexible_boxes#Flex_Item_Considerations

###Flexible Box Properties

Properties not affecting flexible boxes Flex box에서 무시 되는 속성들

Flex box가 다른 레이아웃 알고리즘을 사용하기 때문에 일부 속성들은 Flex container 에서 무시됩니다.

* column-* properties of the multiple column module have no effect on a flex item.
* clear has no effect on a flex item.
* float causes the display property of the element to compute to block.
* vertical-align has no effect on the alignment of flex items.











