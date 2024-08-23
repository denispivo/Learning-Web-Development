## TAGS (Exercise 2 of 11)

HTML uses special bits of programming language called tags to let the
browser know how a webpage should look. The tags usually come in pairs: an
opening tag to tell the browser when to start doing something, and an
ending tag to tell the browser when to stop doing something. There are
many different kinds of tags, and each one has a different purpose.

Let's think of tags like it's some kind of selection tool in text editors.
In text editor, such as Microsoft Office Word or Writer, if you want to
make text bold you select a part of text and click corresponding button
(b). In HTML, you have tags for that reason.

                ┌── a "selected" text ──┐
                ↓                       ↓
Lorem ipsum <tagname>dolor sit amet</tagname>, consectetur adipisicing elit.

Opening tags have a keyword, such as p, surrounded by angle brackets (<
and >). For example, the tag <code><p></code> tells the browser the start a new
paragraph. Ending tags look almost exactly the same, only they have a
forward slash (/) added just before the keyword. For example, the tag <code></p></code>
tells the browser to end a paragraph.

<p>this is a paragraph</p>

  A small number of tags, like <code><br></code>, <code><img></code> and <code><hr></code>, can be used without an
  ending tag. Here is what these tags do:

   » <code><br></code> - produces a line break in text (carriage-return). It is useful
     for writing a poem or an address, where the division of lines is
     significant.
   » <code><img></code> — represents an image in the document. We will consider this tag
     later.
   » <code><hr></code> — represents a thematic break between paragraph-level elements. In
     previous versions of HTML, it represented a horizontal rule. It may
     still be displayed as a horizontal rule in visual browsers.

  You could use them like this:

     <p>first paragraph</p>
     <hr>
     <p>second paragraph</p>