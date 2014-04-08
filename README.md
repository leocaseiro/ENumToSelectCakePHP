ENumToSelectCakePHP
===================

Form Helper: Enum Fields to Select Boxes

Based on http://bakery.cakephp.org/articles/christian.kilb/2010/09/09/form-helper-enum-fields-to-select-boxes, re-builded following the theotherdy's instructions.

Installation:
===================
## Save on
   /app/View/Helpers/Form2Helper.php

## Add in your Controller:

	public $helpers = array('Form2');
	
## Usage on View:

  <?php
    //Note you might use Form2 intead of Form
    echo $this->Form->create('YourModel');
		echo $this->Form2->input('YourModel.your_field', array('type' => 'select')); //For select field (Default)
		echo $this->Form2->input('YourModel.your_field', array('type' => 'radio')); //For radio field
		echo $this->Form->end('Submit');
	?>
