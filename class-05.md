# Images, Color, Text


## Images

In order to add images to your web page, you have to use the **< img >** tag. Unlike most elements, the image tags is an empty element, meaning it does not have a closing tag. However, you do have to include two attributes with it when you use it. The first attribute you have to use is the **src** attribute. This attribute lets the web browser know where the image can be found. Usually, this will be a relative URL, which will be pointing to an image on your own site. After the src attribute, you also want to have an **alt** attribute within the image tag. This attribute is a description of the image, if you cannot see the image. You also have the ability to use a title attribute as well, which will provide additional information about the image, however, in most cases web browsers will display that contents of that same attribute in a tooltip, whenever the user hovers over the image. 

**< img src=“image/locatio.jpg”  alt=“a picture used in an example”  title=“the image can be sourced from many sites” >**

There are three main formats in which you can save an image: JPEG, GIF, and PNG. Whenever you are using an image with many different colors in it, it would be best to use a JPEG. Whenever you are using an image that is filled with a flat color, which is an area filled with exactly the same color, such as what you may see in logos, illustrations or diagrams, then it would be best to save that image as a GIF or PNG. *(Duckett, Jon, HTML & CSS: design and build websites, pp. 94-125 2011.)*

## Color 

Color properties through CSS enable you to set the color of many things on your web page. If you wish to make a specific text a certain color, you can do so with the following: RGB values, Hex code, and Color names. RGB values  are in relation to how much red, blue and green are used to make it up. Hex Codes are six digit codes, which represent the amount of red, blue, or green in a color and has a pound symbol before it. Color names are a selection of 147 predefined color names that your web browser recognizes. Here are examples of the three color properties:

RGB : rgb (120, 200, 80)

Hex Codes:  #ff4f90

Color Names: SkyBlue

Your computer screen displays different colors through the use of pixels, and the different colors you computer screen can display is created by mixing three colors: red, blue, and green. In order to find the color that you specifically want, you can use a tool called a color picker. Most image editing programs have this tool, and can assist you in getting the specific color you want. CSS3 introduces a property known as opacity. This property enables you to specify the opacity or opaqueness  of an element out any of its child elements. The RGBA property within CSS3 enables you to pick a color just like you would with regular RGB; however, it allows you to add opacity or opaqueness  to the color. HSL and HSLA  color properties within CSS3 enable you to adjust things such as the Hue, Saturation, Lightness and Alpha, when choosing your colors. Keep in mind that older browsers do not recognize HSL and HSLA values, so it is best to add an extra rule which specifies the color using hex code. *(Duckett, Jon, HTML & CSS: design and build websites, pp. 246-263 2011.)*


## Text

Within CSS you are able to adjust the font using the font size property. There are multiple way in which you can choose the size of a font. The most commonly used ways are: pixels, percentages, and ems. Pixels are used to adjust font size, because they enable web designers to have very precise control over how much space their text takes. If you wish to use this method of control, the number of pixels that you choose will have a px after them. If you adjust your font size using percentages, you would enter a number with a % symbol after you enter the number. Just for reference, the default size of text in most browsers is 16px, and a size of 75% would be the same equivalent as 12px, and a 200% would be the same equivalent as 32px. An em is the equivalent to how wide the letter m is. 

A font face enables you to use a font, even if it isn’t installed on the computer of the person browsing your site. This technique makes it possible to download a version of font to a user’s computer, that doesn’t exist as a default on it. When you add font to your style sheet, you use the @font face rule. The font family names the font specifically, this name can be used as a value of the font family property in the rest of the style sheet. The src is the path of the font. In order to make this work on all browsers you will have to specify paths to a few different versions of the font. Format specifies the format that the font is supplied in. *(Duckett, Jon, HTML & CSS: design and build websites, pp. 264-299 2011.)*


## JPEG vs PNG vs GIF

The three most commonly used image formats in both websites and phone apps are JPEG, PNG and GIF. Together these three formats make up more than 95% of all images loaded onto websites. Generally speaking you would use JPEG format for images that have a natural scene or an image where the variation in color and intensity is smooth. PNG format is used for images that need transparency, or for images with text and objects with sharp contrasts edges, such as logos. GIF format is used for animations. *(Nanwani, Rahul, JPEG vs PNG vs GIF - which image format to use and when?, 2016NOV13)*