**This is not pushed yet**

**Max stylesheet size:** 10,000 characters [i]'ish[/i]

* Nesting
  ```CSS
  #content {
  	background: #1a1a1a;
  	
  	#inner {
  		opacity: .98;
  	}
  	
  	.post {
  		
  		&_author {
  			background: red;
  		}
  		
  		> .bit {
  			background: blue;
  			
  			&:hover {
  				background: purple;
  			}
  		}
  	}
  }
  ```

* Variables
  ```CSS
  $bg: #1a1a1a;
  
  .username {
       background: $bg;
  }
  ```

* Colors
  ```CSS
  $bg: #1a1a1a;
  
  .username {
       background: lighten($bg, 20%); /* Lightens the color by 20% */
       background: darken($bg, 10%); /* Darkens the color by 10% */
  }
  ```

* Mixing
  ```CSS
  .trow {
      border-top: 1px solid #303030;
      border-bottom: 1px solid #0f0f0f;
  }
  
  table th > td {
      background: #1a1a1a;
      .trow;
  }
  
  table tr > td {
      background: #252525;
      .trow;
  }
  ```

**Global variables**:
  * $theme_color: Your theme color when saving
