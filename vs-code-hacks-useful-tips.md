# Shortcuts ⌨️✅

- `command + d` locate and edit duplicate items, perfect for editing the same variables on the same page at once
- `shift + option + ↓` duplicate the current line of code

</br>

# Autocomplete 🤖🦾
💡 Press `tab` or `enter` at the end

### HTML 
  
- Use `.` to attach a class to the tag `div.awesome-class` converts to: </br>
    ```html
      <div class="awesome-class"></div>
    ```

- Use `#` to attach an id to the tag `div#specific-id` converts to: </br>
    ```html
      <div id="specific-id"></div>
    ```
        
- Use `>` to include a child element `div.parent-class>div.child-class` converts to: </br>
    ```html
      <div class="parent-class">
        <div class="child-class"></div>
      </div>
    ```
        
- Use `*` to create duplicate elements `ul>li*3>button.btn` converts to: </br>
    ```html
      <ul>
        <li><button class="btn"></button></li>
        <li><button class="btn"></button></li>
        <li><button class="btn"></button></li>
      </ul>
    ```
        
- Use `$` to add incrementing numbers `table>tbody>tr>td*5.cell$` converts to: </br> 
    ```html
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

- Use `{}` to add contents between tags `div.your-class{item}` converts to: </br>
    ```html
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
