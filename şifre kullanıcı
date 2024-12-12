package com.example.sifrekullanici;

import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.Toast;

import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity {

    EditText textad;
    EditText textsifre;
    Button buttonsonuc;

    final String kullaniciadi="Alper";
    final String kullanicisifre="123alper";

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        EdgeToEdge.enable(this);
        setContentView(R.layout.activity_main);
        ViewCompat.setOnApplyWindowInsetsListener(findViewById(R.id.main), (v, insets) -> {
            Insets systemBars = insets.getInsets(WindowInsetsCompat.Type.systemBars());
            v.setPadding(systemBars.left, systemBars.top, systemBars.right, systemBars.bottom);
            return insets;
        });
        textad=findViewById(R.id.txtAd);
        textsifre=findViewById(R.id.txtSifre);
        buttonsonuc=findViewById(R.id.btnSonuc);
    }
    public void kontrol(View view) {
        String kullaniciadigiris = textad.getText().toString();
        String kullanicisifregiris = textsifre.getText().toString();

        if (kullaniciadi.equals(kullaniciadigiris) && kullanicisifre.equals(kullanicisifregiris)) {
            Toast.makeText(this, "Kullanıcı girişi başarılı", Toast.LENGTH_SHORT).show();
        }
            else {
            Toast.makeText(this, "Kullanıcı girişi başarısız", Toast.LENGTH_SHORT).show();
        }
    }
}
