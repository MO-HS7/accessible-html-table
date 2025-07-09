# accessible-html-table
**Q2: What is Accessibility in web, and why is it important in web programming?**  
**Accessibility** (a11y) means designing and developing websites that can be used by everyone, including people with disabilities (such as visual, auditory, motor, or cognitive impairments).  

It is important because:

- It ensures equal access to information and functionality for all users.  
- It improves usability for everyone, not just people with disabilities.  
- It helps meet legal requirements and international standards (like WCAG).  
- It enhances SEO and site structure.  
- It promotes inclusion and social equity.

---

**What is the `scope` attribute, and how does it support accessibility?**

The `scope` attribute is used in HTML tables with `<th>` (table header) elements to define the set of data cells that the header relates to. It helps screen readers understand the table structure and navigate it more effectively.

- `scope="col"`: Header applies to a column.  
- `scope="row"`: Header applies to a row.  
- `scope="colgroup"` / `scope="rowgroup"`: Applies to a group of columns or rows.

---

**Example: Accessible HTML Table using `scope` Attribute**

```html
<table>
  <caption>Student Grades</caption>
  <thead>
    <tr>
      <th scope="col">Name</th>
      <th scope="col">Age</th>
      <th scope="col">Grade</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">Ahmed</th>
      <td>15</td>
      <td>90</td>
    </tr>
    <tr>
      <th scope="row">Sarah</th>
      <td>16</td>
      <td>95</td>
    </tr>
  </tbody>
</table>
```

This code uses semantic markup and the `scope` attribute to ensure screen readers correctly associate headers with their corresponding data cells, improving accessibility for users with visual impairments.
