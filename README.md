# MainActivity.kt
 تطبيق يحسب رقمين ويقسمهما عل مليون
 
 
package com.example.myapplication

import android.support.v7.app.AppCompatActivity
import android.os.Bundle
import kotlinx.android.synthetic.main.activity_main.*

class MainActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        btn.setOnClickListener({
            //result Ø§Ù„Ù†ØªÙŠØ¬Ø©
            val number1:Int=number1.text.toString().toInt()
            val number2:Int=number2.text.toString().toInt()
            result.text="your result is"
            val result=1000000/(number1+number2)
        })
    }
}
