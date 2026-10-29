Homework 2: Mankato Maker Club (invented club)
Sasmit Tomar, CIS 483/583
 
Semantic choice 1: I used < aside > for the contact block on the home page and the help block on the events page. This content supports the page but is not part of the main story, so < aside > tells screen readers and search engines that it is secondary information, which a generic < div > would not do.

Semantic choice 2: I wrapped each radio group and checkbox group in a < fieldset > with a < legend >. The legend gives screen reader users the group question (for example, "Membership type") before each option, and it keeps related controls together in the markup.

Bug: While testing the form in the browser with DevTools open, I found that the optional phone field silently rejected a number typed without dashes (5075550123), and the format hint only appeared after a failed submit. I fixed it by adding placeholder="507-555-0123" so the required format shows before the user types, and I kept the title attribute for the error message.

Both pages passed validator.w3.org with no errors or warnings (screenshots included), and the console shows zero errors with all images loading.
Source cited: MDN Web Docs for HTML element and form validation reference.
