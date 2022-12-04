# VS Code Hacks & Useful Tips

## Shortcuts ✅⌨️

- `command + d` locate and edit duplicate items, perfect for editing the same variables on the same page at once
- `shift + option + ↓` duplicate the current line of code

</br>

## Autocomplete 🤖🦾
💡 Press `tab` or `enter` at the end

### HTML 
  
- Use `.` to attach a class to the tag
    ```html
      <!-- div.awesome-class -->
      <div class="awesome-class"></div>
    ```

- Use `#` to attach an id to the tag
    ```html
      <!-- div#specific-id -->
      <div id="specific-id"></div>
    ```
        
- Use `>` to include a child element
    ```html
      <!-- div.parent-class>div.child-class -->
      <div class="parent-class">
        <div class="child-class"></div>
      </div>
    ```
        
- Use `*` to create duplicate elements
    ```html
      <!-- ul>li*3>button.btn -->
      <ul>
        <li><button class="btn"></button></li>
        <li><button class="btn"></button></li>
        <li><button class="btn"></button></li>
      </ul>
    ```
        
- Use `$` to add incrementing numbers
    ```html
      <!-- table>tbody>tr>td*5.cell$ -->
      <table>
        <tbody>
          <tr>
            <td class="cell1"></td>
            <td class="cell2"></td>
            <td class="cell3"></td>
            <td class="cell4"></td>
            <td class="cell5"></td>
          </tr>
        </tbody>
      </table>
    ```

- Use `{}` to add contents between tags
    ```html
      <!-- div.your-class{item} -->
      <div class="your-class">item</div>
    ```
        
### CSS
💡 Use initial to find attributes, type value and units to autocomplete
    
- `m10px` `pl5rem` `bc#fff` converts to: </br>
    ```css
      margin: 10px;
      padding-left: 5rem;
      background-color: #fff;
    ```
