 import java.awt.*; 															// импорт пакета awt
 import java.awt.event.ActionEvent; 											// импорт пакета awt.event.ActionEvent
 import java.awt.event.ActionListener; 										// импорт пакета awt.event.ActionListener
 import java.awt.event.ItemEvent; 											// импорт пакета awt.event.ItemEvent
 import java.awt.event.ItemListener; 										// импорт пакета event.ItemListener
 import java.text.*; 														// импорт пакета text
 import javax.swing.*; 														// импорт пакета swing
 import javafx.*;															// импорт пакета javafx
 public class nds															// открытый класс "nds"
 {																			// открывающий символ
 	private JLabel log;														// добавление часного модуля log типа Jlabel(надпись)
 	private JLabel log11;													// добавление часного модуля log11 типа Jlabel(надпись)
 	private JLabel log1;													// добавление часного модуля log1 типа Jlabel(надпись)
     private JLabel log2;													// добавление часного модуля log2 типа Jlabel(надпись)
     private JLabel log3;													// добавление часного модуля log3 типа Jlabel(надпись)
     private JLabel log4;													// добавление часного модуля log4 типа Jlabel(надпись)
     private JLabel log5;													// добавление часного модуля log5 типа Jlabel(надпись)
     private JLabel log6;													// добавление часного модуля log6 типа Jlabel(надпись)
     private JLabel log7;													// добавление часного модуля log7 типа Jlabel(надпись)
     private JLabel log8;													// добавление часного модуля log8 типа Jlabel(надпись)
     private JLabel rubl1;													// добавление часного модуля rubl1 типа Jlabel(надпись)
     private JLabel rubl2;													// добавление часного модуля rubl2 типа Jlabel(надпись)
     private JLabel rubl3;													// добавление часного модуля rubl3 типа Jlabel(надпись)
     private JLabel rubl4;													// добавление часного модуля rubl4 типа Jlabel(надпись)
     private JLabel result;													// добавление часного модуля result типа Jlabel(надпись)
     private JTextField text1;												// добавление часного модуля text1 типа JTextField(текстовое поле)
     private JTextField text2;												// добавление часного модуля text2 типа JTextField(текстовое поле)
     private JTextField text3;												// добавление часного модуля text3 типа JTextField(текстовое поле)
     private JTextField text4;												// добавление часного модуля text4 типа JTextField(текстовое поле)
     private JComboBox comboBox;												// добавление часного модуля comboBox типа JComboBox(выпадающий список)
     private JComboBox comboBox1;											// добавление часного модуля comboBox1 типа JComboBox(выпадающий список)
     private JComboBox comboBox2;											// добавление часного модуля comboBox2 типа JComboBox(выпадающий список)
     private JComboBox comboBox3;											// добавление часного модуля comboBox3 типа JComboBox(выпадающий список)
     private JComboBox comboBox4;											// добавление часного модуля comboBox4 типа JComboBox(выпадающий список)
     private JButton Button1;												// добавление часного модуля Button1 типа JButton(кнопка)
     private JButton Button2;												// добавление часного модуля Button2 типа JButton(кнопка)
     private JFrame mainFrame;												// добавление часного модуля mainFrame типа JFrame(форма)    
     nds() {																	// начало класса
 //colors
 Color back = new Color(245,245,220);										// присвоение переменной back цвета
 Color font = new Color(132,132,130);										// присвоение переменной font цвета
 Color button = new Color(255, 229, 180);									// присвоение переменной button цвета
 //labels  
         log = new JLabel("Программа для расчета НДС");						// создание объекта log типа  Jlable
        	Font head = new Font("Verdana", Font.BOLD, 12);						// присвоение переменной head стиля текста
        	log.setFont(head);													// присвоение объекту log стиля текста равному значению переменной head
         log11 = new JLabel("Введите цену товара в поле");					// создание объекта log11 типа  Jlable
         log1 = new JLabel("Цена товара введена");							// создание объекта log1 типа  Jlable
     	log2 = new JLabel("Вид торговли");									// создание объекта log2 типа  Jlable
         log3 = new JLabel("Наличие комплекта документов");					// создание объекта log3 типа  Jlable
         log4 = new JLabel("Реализация специальных товаров");				// создание объекта log4 типа  Jlable
         log5 = new JLabel("Налогоплательщик это");							// создание объекта log5 типа  Jlable
         log6 = new JLabel("Сумма с НДС");       							// создание объекта log6 типа  Jlable
         log6.setVisible(false);												// задаем значение свойства отображения объекта log6 = невидимый
         log7 = new JLabel("Сумма без НДС");        							// создание объекта log7 типа  Jlable
         log7.setVisible(false);												// задаем значение свойства отображения объекта log7 = невидимый
         log8 = new JLabel("НДС");              								// создание объекта log8 типа  Jlable
         log8.setVisible(false);												// задаем значение свойства отображения объекта log8 = невидимый
        	Font font1 = new Font("", Font.BOLD, 13);							// присвоение переменной font1 стиля текста
        	log6.setFont(font1);												// присвоение объекту log6 стиля текста равному значению переменной font1
        	log7.setFont(font1);												// присвоение объекту log7 стиля текста равному значению переменной font1
        	log8.setFont(font1);												// присвоение объекту log8 стиля текста равному значению переменной font1
         rubl1 = new JLabel("руб");											// создание объекта rubl1 типа  Jlable
         rubl2 = new JLabel("руб");											// создание объекта rubl2 типа  Jlable
         rubl2.setVisible(false);											// задаем значение свойства отображения объекта rubl2 = невидимый
         rubl3 = new JLabel("руб");											// создание объекта rubl3 типа  Jlable
         rubl3.setVisible(false);											// задаем значение свойства отображения объекта rubl3 = невидимый
         rubl4 = new JLabel("руб");											// создание объекта rubl4 типа  Jlable
         rubl4.setVisible(false);											// задаем значение свойства отображения объекта rubl4 = невидимый
         result = new JLabel("Введите необходимые данные");					// создание объекта result типа  JLabel
         result.setForeground(Color.RED);									// установка цвета текста Jlabel result
 //buttons
         Button1 = new JButton("Расчитать");									// создание объекта Button3 типа  JButton
       	Button1.setEnabled(false);											// перевод кнопки Button3 в не доступное состояние (для нажатия) методом setEnabled
       	Button2 = new JButton("Заново");									// создание объекта Button4 типа  JButton
       	Button2.setVisible(false);											// задаем значение свойства отображения объекта Button2 = невидимый
       	Button1.setBackground(button);										// присвоение объекту Button1 цвета фона равному значению переменной button
       	Button2.setBackground(button);										// присвоение объекту Button2 цвета фона равному значению переменной button
 // comboboxes
     	String[] items = {													// создание строк текста 			
     			"",															// первая строка
                 "Физическое лицо",											// вторая строка
                 "Индивидуальный предприниматель"							// третья строка
             };																// конец создания строк			
     	JComboBox editComboBox = new JComboBox(items);						// объединение строк в выпадающий список                        
         comboBox = new JComboBox(items);									// создание объекта  comboBox типа  JComboBox
         comboBox.setEnabled(false);											// перевод выбора из списка comboBox в недоступное состояние (для нажатия) методом setEnabled
       	String[] items1 = {													// создание строк текста 			
     			"",															// первая строка
     			"С НДС",													// вторая строка
     			"Без НДС"													// третья строка
             };																// конец создания строк	
       	JComboBox editComboBox1 = new JComboBox(items1);					// объединение строк в выпадающий список  
       	comboBox1 = new JComboBox(items1);									// создание объекта  comboBox1 типа  JComboBox
       	String[] items2 = {													// создание строк текста 			
     			"",															// первая строка
     			"Местная",													// вторая строка
     			"Экспорт"													// третья строка
             };																// конец создания строк	
       	JComboBox editComboBox2 = new JComboBox(items2);					// объединение строк в выпадающий список  
       	comboBox2 = new JComboBox(items2);									// создание объекта  comboBox2 типа  JComboBox
       	comboBox2.setEnabled(false);										// перевод выбора из списка comboBox2 в недоступное состояние (для нажатия) методом setEnabled   	
       	String[] items3 = {													// создание строк текста 			
     			"",															// первая строка
     			"Есть",														// вторая строка
     			"Отсутствует"												// третья строка
             };																// конец создания строк	
       	JComboBox editComboBox3 = new JComboBox(items3);					// объединение строк в выпадающий список
       	comboBox3 = new JComboBox(items3);									// создание объекта  comboBox3 типа  JComboBox
       	comboBox3.setEnabled(false);										// перевод выбора из списка comboBox3 в недоступное состояние (для нажатия) методом setEnabled      	
       	String[] items4 = {													// создание строк текста 			
     			"",															// первая строка
     			"Да",														// вторая строка
     			"Нет"														// третья строка
             };																// конец создания строк	
       	JComboBox editComboBox4 = new JComboBox(items4);					// объединение строк в выпадающий список
       	comboBox4 = new JComboBox(items4);									// создание объекта  comboBox4 типа  JComboBox
       	comboBox4.setEnabled(false);										// перевод выбора из списка comboBox4 в недоступное состояние (для нажатия) методом setEnabled
 	    comboBox.setBackground(button);										// присвоение объекту comboBox цвета фона равному значению переменной button
 		comboBox1.setBackground(button);									// присвоение объекту comboBox1 цвета фона равному значению переменной button
 		comboBox2.setBackground(button);									// присвоение объекту comboBox2 цвета фона равному значению переменной button
 		comboBox3.setBackground(button);									// присвоение объекту comboBox3 цвета фона равному значению переменной button
 		comboBox4.setBackground(button);									// присвоение объекту comboBox4 цвета фона равному значению переменной button
 //textfields
         text1 = new JTextField("");											// создание объекта text1 типа  JTextField
         text1.setHorizontalAlignment(JTextField.RIGHT);						// установка выравнивания содержания метки вдоль X осей
         text2 = new JTextField("");											// создание объекта text2 типа  JTextField
         text2.setEditable(false);											// запрет редактирования поля  text2
         text2.setVisible(false);											// задаем значение свойства отображения объекта text2 = невидимый
         text2.setHorizontalAlignment(JTextField.RIGHT);						// установка выравнивания содержания метки вдоль X осей
         text3 = new JTextField("");											// создание объекта text3 типа  JTextField
         text3.setEditable(false);											// запрет редактирования поля  text3		
         text3.setVisible(false);											// задаем значение свойства отображения объекта text3 = невидимый
         text3.setHorizontalAlignment(JTextField.RIGHT);						// установка выравнивания содержания метки вдоль X осей
         text4 = new JTextField("");											// создание объекта text4 типа  JTextField
         text4.setEditable(false);											// запрет редактирования поля  text4		
         text4.setVisible(false);											// задаем значение свойства отображения объекта text4 = невидимый
         text4.setHorizontalAlignment(JTextField.RIGHT);						// установка выравнивания содержания метки вдоль X осей
 		text1.setBackground(button);										// присвоение объекту text1 цвета фона равному значению переменной button
 		text2.setBackground(button);										// присвоение объекту text2 цвета фона равному значению переменной button
 		text3.setBackground(button);										// присвоение объекту text3 цвета фона равному значению переменной button
 		text4.setBackground(button);										// присвоение объекту text4 цвета фона равному значению переменной button
  //action listeners       
         ActionListener again = new ActionListener() {						// объявление слушателя again (обработку события нажатия на кнопку)
             @Override														// добавление аннотации Override
              public void actionPerformed(ActionEvent ar) {					// объявление метода actionPerformed
                 comboBox.setSelectedItem("");								// присвоение объекту comboBox значения равного пустому полю
                 comboBox1.setSelectedItem("");								// присвоение объекту comboBox1 значения равного пустому полю
                 comboBox2.setSelectedItem("");								// присвоение объекту comboBox2 значения равного пустому полю
                 comboBox3.setSelectedItem("");								// присвоение объекту comboBox3 значения равного пустому полю
                 comboBox4.setSelectedItem("");								// присвоение объекту comboBox4 значения равного пустому полю
             	comboBox1.setEnabled(true);									// перевод выбора из списка comboBox1 в доступное состояние (для нажатия) методом setEnabled	
                	Button1.setEnabled(false);									// перевод кнопки Button3 в не доступное состояние (для нажатия) методом setEnabled
             	Button2.setEnabled(false);									// перевод кнопки Button4 в не доступное состояние (для нажатия) методом setEnabled
                 text1.setEnabled(true);										// разрешение редактирования поля  text1
                 log11.setVisible(true);										// задаем значение свойства отображения объекта log11 = видимый
                 log1.setVisible(true);										// задаем значение свойства отображения объекта log1 = видимый
                 log2.setVisible(true);										// задаем значение свойства отображения объекта log2 = видимый
                 log3.setVisible(true);										// задаем значение свойства отображения объекта log3 = видимый
                 log4.setVisible(true);										// задаем значение свойства отображения объекта log4 = видимый
                 log5.setVisible(true);										// задаем значение свойства отображения объекта log5 = видимый
                 text1.setVisible(true);										// задаем значение свойства отображения объекта text1 = видимый
                 comboBox.setVisible(true);									// задаем значение свойства отображения объекта comboBox = видимый
                 comboBox1.setVisible(true);									// задаем значение свойства отображения объекта comboBox1 = видимый
                 comboBox2.setVisible(true);									// задаем значение свойства отображения объекта comboBox2 = видимый
                 comboBox3.setVisible(true);									// задаем значение свойства отображения объекта comboBox3 = видимый
                 comboBox4.setVisible(true);									// задаем значение свойства отображения объекта comboBox4 = видимый
                 Button1.setVisible(true);									// задаем значение свойства отображения объекта Button1 = видимый
                 rubl1.setVisible(true);										// задаем значение свойства отображения объекта rubl1 = невидимый
                 Button2.setVisible(false);									// задаем значение свойства отображения объекта Button2 = невидимый
                 log6.setVisible(false);										// задаем значение свойства отображения объекта log6 = невидимый
                 log7.setVisible(false);										// задаем значение свойства отображения объекта log7 = невидимый
                 log8.setVisible(false);										// задаем значение свойства отображения объекта log8 = невидимый
                 text2.setVisible(false);									// задаем значение свойства отображения объекта text2 = невидимый
                 text3.setVisible(false);									// задаем значение свойства отображения объекта text3 = невидимый
                 text4.setVisible(false);									// задаем значение свойства отображения объекта text4 = невидимый
                 rubl2.setVisible(false);									// задаем значение свойства отображения объекта rubl2 = невидимый
                 rubl3.setVisible(false);									// задаем значение свойства отображения объекта rubl3 = невидимый
                 rubl4.setVisible(false);									// задаем значение свойства отображения объекта rubl4 = невидимый
                 result.setText("Введите необходимые данные");				// присваиваем значению объекта result текстовое значение "Введите необходимые данные"
             }																// конец метода actionPerformed    
         };																	// конец работы слушателя again
         final ActionListener bnds1 = new ActionListener() {					// объявление слушателя bnds1 (обработку события нажатия на кнопку)
             @Override														// добавление аннотации Override
              public void actionPerformed(ActionEvent calc) {				// объявление метода actionPerformed	
                try {														// объявление оператора try (попытка выполнить действия)
                 double cost2 = Double.parseDouble(text1.getText()); 		// определение типа(Double) переменной(cost2) методом parseDouble,присваиваение переменной cost2 введенного значения из text1
                 double nds2 = cost2 * 0.1;									// определение типа переменной(nds2), присваиваение nds2 значение выражения
                 double summas2 = cost2 + nds2;								// определение типа переменной(summas2), присваиваение summas2 значение выражения
                 double summabez2 = cost2; 									// определение типа переменной(summabez2), присваиваение summabez2 значение выражения
                 NumberFormat na = NumberFormat.getInstance();				// присвоение класса NumberFormat переменной na методом getInstance
                 na.setMaximumFractionDigits(2);   							// ограничение количества цифр после запятой до 2-ух
                 text2.setText(""+na.format(summas2));						// вывод значения summas2 в поле text2, используя метод setText и ограничение количества цифр после запятой методом format
                 text3.setText(""+na.format(summabez2));						// вывод значения summabez2 в поле text3, используя метод setText и ограничение количества цифр после запятой методом format
                 text4.setText(""+na.format(nds2));							// вывод значения nds2 в поле text4, используя метод setText и ограничение количества цифр после запятой методом format
                 result.setText("");											// вывод текста "" в поле  result, используя метод setText
                 log11.setVisible(false);									// задаем значение свойства отображения объекта log11 = невидимый
                 log1.setVisible(false);										// задаем значение свойства отображения объекта log1 = невидимый
                 log2.setVisible(false);										// задаем значение свойства отображения объекта log2 = невидимый
                 log3.setVisible(false);
