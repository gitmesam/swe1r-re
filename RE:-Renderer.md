# Prepare for draw

```C
//----- (0048DF30) --------------------------------------------------------
unsigned int __cdecl sub_48DF30(unsigned int a1, float *a2)
{
  unsigned int result; // eax
  float *v3; // esi
  float v4; // eax
  int v5; // ecx
  int v6; // ecx
  int v7; // ecx
  int v8; // ecx
  int v9; // eax
  int v10; // eax
  int v11; // ecx
  int v12; // edx
  int v13; // edi
  int v14; // edi
  unsigned int v15; // ecx
  __int16 v16; // dx
  unsigned int v17; // ebx
  int v18; // edx
  int v19; // edi
  char *v20; // ecx
  double v21; // st7
  float v22; // ST2C_4
  bool v25; // zf
  double v26; // st7
  float v27; // eax
  float v28; // edx
  float v29; // ST4C_4
  signed int v32; // edx
  float v33; // ST4C_4
  signed int v36; // edi
  float v37; // ST4C_4
  signed int v40; // ebx
  float v41; // ST4C_4
  int v44; // edx
  unsigned int v45; // edx
  float v46; // ST44_4
  char v49; // dl
  float v50; // ST44_4
  signed int v53; // edi
  float v54; // ST44_4
  unsigned int v57; // eax
  int v58; // edi
  signed __int16 v59; // dx
  _WORD *v60; // eax
  int v61; // eax
  unsigned int v62; // ebx
  int v63; // [esp+0h] [ebp-68h]
  int v64; // [esp+4h] [ebp-64h]
  int v65; // [esp+10h] [ebp-58h]
  int v66; // [esp+14h] [ebp-54h]
  __int16 v67; // [esp+18h] [ebp-50h]
  unsigned int v68; // [esp+1Ch] [ebp-4Ch]
  signed __int16 v69; // [esp+1Ch] [ebp-4Ch]
  unsigned int v70; // [esp+20h] [ebp-48h]
  int v71; // [esp+20h] [ebp-48h]
  signed int v72; // [esp+24h] [ebp-44h]
  int v73; // [esp+2Ch] [ebp-3Ch]
  signed __int16 v74; // [esp+2Ch] [ebp-3Ch]
  int v75; // [esp+30h] [ebp-38h]
  int v76; // [esp+30h] [ebp-38h]
  int v77; // [esp+34h] [ebp-34h]
  int v78; // [esp+38h] [ebp-30h]
  int v79; // [esp+3Ch] [ebp-2Ch]
  unsigned int v80; // [esp+40h] [ebp-28h]
  int v81; // [esp+44h] [ebp-24h]
  int v82; // [esp+48h] [ebp-20h]
  int v83; // [esp+4Ch] [ebp-1Ch]
  float v84; // [esp+50h] [ebp-18h]
  float v85; // [esp+54h] [ebp-14h]
  float v86; // [esp+58h] [ebp-10h]
  int v87; // [esp+5Ch] [ebp-Ch]
  int v88; // [esp+60h] [ebp-8h]
  int v89; // [esp+64h] [ebp-4h]
  int v90; // [esp+74h] [ebp+Ch]

  sub_48B260(
    *(float *)(dword_DF7F2C + 56),
    *(float *)(dword_DF7F2C + 64),
    *(float *)(*(_DWORD *)(dword_DF7F2C + 72) + 4),
    *(float *)(*(_DWORD *)(dword_DF7F2C + 72) + 8));
  sub_49EA00();
  result = a1;
  v80 = 0;
  if ( a1 )
  {
    v3 = a2;
    do
    {
      v4 = *v3;
      v90 = 19;
      v66 = *(_DWORD *)v3;
      v64 = *(_DWORD *)v3 & 2;
      if ( *(_DWORD *)v3 & 2 )
        v90 = 531;
      if ( LOBYTE(v4) & 4 )
      {
        v5 = v90;
        BYTE1(v5) |= 8u;
        v90 = v5;
      }
      if ( LOBYTE(v4) & 8 )
      {
        v6 = v90;
        BYTE1(v6) |= 0x10u;
        v90 = v6;
      }
      if ( !(LOBYTE(v4) & 0x10) )
      {
        v7 = v90;
        LOBYTE(v7) = v90 | 0x80;
        v90 = v7;
      }
      if ( LOBYTE(v4) & 0x20 )
      {
        v8 = v90;
        BYTE1(v8) |= 0x20u;
        v90 = v8;
      }
      if ( BYTE1(v4) & 3 )
      {
        v9 = v90;
        BYTE1(v9) |= 0x80u;
        v90 = v9;
      }
      v10 = *((_DWORD *)v3 + 7);
      v63 = *((_DWORD *)v3 + 7);
      if ( v10 )
      {
        v11 = *(_DWORD *)(v10 + 124);
        if ( v11 )
        {
          v12 = v90;
          BYTE1(v12) |= 4u;
          v90 = v12;
        }
        v13 = *(_DWORD *)(v10 + 144);
        sub_48E5F0(*(_DWORD **)(v10 + 144), v11);
        v65 = *(_DWORD *)(v13 + 128);
      }
      else
      {
        v65 = 0;
      }
      v14 = 0;
      v15 = 0;
      v83 = 0;
      dword_A530D0 = 0;
      dword_5430C0 = *(_DWORD *)(*(_DWORD *)(dword_DF7F2C + 72) + 4);
      do
      {
        v68 = *((_DWORD *)v3 + 2);
        dword_5430C4 = *((_DWORD *)v3 + 4);
        dword_AF30DC = *((_DWORD *)v3 + 6);
        v16 = v15;
        v67 = v15;
        v72 = *((_DWORD *)v3 + 1);
        if ( v72 >= dword_ECC424 )
          v72 = dword_ECC424;
        v17 = 0;
        v70 = 0;
        if ( v68 ) {
          v73 = 0;
          v75 = 0;



          while ( 1 ) {
            v18 = v75 + dword_5430C4;
            v19 = dword_AF30DC + v73;

            // Generate output address (v15 = vertex index, 32 = stride)
            v20 = (char *)&unk_B6B0E8 + 32 * v15;

            // Copy X?
            *(_DWORD *)v20 = *(_DWORD *)(v75 + dword_5430C4);

            // Copy Y?
            *((_DWORD *)v20 + 1) = *(_DWORD *)(v18 + 4);

            // Copy RHW?
            if ( *(float *)(v18 + 8) == 0.0 ) {
              v21 = 0.0;
            } else {
              v21 = (2.0 - *(float *)(v18 + 8) * COERCE_FLOAT(2130706432 - *(_DWORD *)(v18 + 8)))
                  * COERCE_FLOAT(2130706432 - *(_DWORD *)(v18 + 8));
            }

            // Copy Z?
            if ( *(float *)(v18 + 8) == *(float *)&dword_5430C0 ) {
              *((_DWORD *)v20 + 2) = 0;
            } else {
              *((float *)v20 + 2) = 1.0 - v21 * *(float *)&dword_5430C0;
            }
            *((float *)v20 + 3) = v21;

            // Probably something to do with colors or alpha blending
            if ( v66 & 0x200 ) {
              if ( *(float *)(v18 + 8) > (double)*(float *)&flt_EC8578 ) {
                if ( *(float *)(v18 + 8) < (double)*(float *)&flt_EC857C ) {
                  v22 = (1.0 - (*(float *)(v18 + 8) - *(float *)&flt_EC8578) * flt_EC8574) * 255.0;
                  _ST7 = v22;
                  __asm { frndint }
                  v79 = (signed int)_ST7;
                  *((_DWORD *)v20 + 5) = ((signed int)_ST7 << 24) | 0xFFFFFF;
                } else {
                  *((_DWORD *)v20 + 5) = 0x00FFFFFF;
                }
              } else{
                *((_DWORD *)v20 + 5) = 0xFFFFFFFF;
              }
            }
            if ( v72 <= 0 )
              goto LABEL_43;
            if ( v72 > 2 )
              break;
            v27 = *(float *)(v19 + 4);
            v26 = *(float *)(v19 + 12);
            v86 = *(float *)v19;
            v28 = *(float *)(v19 + 8);
            v85 = v27;
            v84 = v28;
LABEL_44:
            v86 = MIN(v86, 1.0);
            v85 = MIN(v85, 1.0);
            v84 = MIN(v84, 1.0);
            v26 = MIN(v26, 1.0);

            // Convert some colors from float to integer
            if ( v64 ) {
              v29 = v26 * 255.0;
              _ST7 = v29;
              __asm { frndint }
              v89 = (signed int)_ST7;
              v32 = (signed int)_ST7;
              v33 = v86 * 255.0;
              _ST7 = v33;
              __asm { frndint }
              v88 = (signed int)_ST7;
              v36 = (signed int)_ST7;
              v37 = v85 * 255.0;
              _ST7 = v37;
              __asm { frndint }
              v82 = (signed int)_ST7;
              v40 = (signed int)_ST7;
              v41 = v84 * 255.0;
              _ST7 = v41;
              __asm { frndint }
              v78 = (signed int)_ST7;
              v17 = v70;
              // This was originally: v45 = ((v40 | ((v36 | (v32 << 8)) << 8)) << 8) | (signed int)_ST7;
              v45 = (v36 << 24) (v36 << 16) | (v40 << 8) | (signed int)ST7;
            }  else {
              v46 = v86 * 255.0;
              _ST7 = v46;
              __asm { frndint }
              v87 = (signed int)_ST7;
              v49 = (signed int)_ST7;
              v50 = v85 * 255.0;
              _ST7 = v50;
              __asm { frndint }
              v81 = (signed int)_ST7;
              v53 = (signed int)_ST7;
              v54 = v84 * 255.0;
              _ST7 = v54;
              __asm { frndint }
              v77 = (signed int)_ST7;
              v45 = (signed int)_ST7 | ((v53 | ((*(_DWORD *)&v49 | 0xFFFFFF00) << 8)) << 8);
            }
            *((_DWORD *)v20 + 4) = v45;
            v75 += 12;

            // Copy U?
            *((float *)v20 + 6) = *(float *)(*((_DWORD *)v3 + 5) + 8 * v17) + v3[14];
            v73 += 16;

            // Copy V?
            *((float *)v20 + 7) = *(float *)(*((_DWORD *)v3 + 5) + 8 * v17 + 4) + v3[15];

            // Generate next index
            v15 = dword_A530D0 + 1;
            ++v17;
            ++dword_A530D0;
            v70 = v17;
            if ( v17 >= v68 ) {
              v16 = v67;
              v14 = v83;
              goto LABEL_57;
            }
          }




          if ( v72 == 3 )
          {
            v25 = *((float*)v3 + 12) == 1.0f;
            v86 = v3[9] + *(float *)v19;
            v85 = v3[10] + *(float *)(v19 + 4);
            v84 = v3[11] + *(float *)(v19 + 8);
            v26 = *(float *)(v19 + 12);
            if ( !v25 )
              v26 = v26 + v3[12];
            goto LABEL_44;
          }
LABEL_43:
          v84 = 1.0;
          v85 = 1.0;
          v86 = 1.0;
          v26 = *(float *)(dword_AF30DC + 12);
          goto LABEL_44;
        }
LABEL_57:
        v57 = *((_DWORD *)v3 + 2);
        if ( v57 <= 3 )
        {
          word_AF30E8[v14] = v16;
          word_AF30EA[v14] = v16 + 1;
          word_AF30EC[v14] = v16 + 2;
          v14 += 3;
          v83 = v14;
        }
        else
        {
          v58 = v57 - 2;
          v59 = 0;
          v71 = v57 - 2;
          v74 = 1;
          v69 = v57 - 1;
          v76 = 0;
          if ( (signed int)(v57 - 2) > 0 )
          {
            v60 = (_WORD *)(2 * v83 + 11481322);
            v83 += v58 + 2 * v71;
            do
            {
              *(v60 - 1) = v67 + v59;
              *v60 = v67 + v74;
              v60[1] = v69 + v67;
              v60 += 3;
              if ( ~(_BYTE)v76 & 1 )
                v59 = v74++;
              else
                v59 = v69--;
              ++v76;
            }
            while ( v76 < v71 );
          }
          v14 = v83;
        }
        v61 = *((_DWORD *)v3 + 18);
        v3 += 16;
        v62 = v80++ + 1;
      }
      while ( v61 + v14 + 2 * v61 - 6 < (unsigned int)dword_52E624
           && v62 < a1
           && v63 == *((_DWORD *)v3 + 7)
           && v66 == *(_DWORD *)v3 );
      sub_48A350(v65, v90, (int)&unk_B6B0E8, v15, (int)word_AF30E8, v14);
      result = a1;
    }
    while ( v80 < a1 );
  }
  return result;
}
```

# Draw function

```C
//----- (0048A350) --------------------------------------------------------
// a1 = texture
// a2 = renderstates
// a3 = vertex pointer
// a4 = vertex count
// a5 = index pointer
// a6 = index count
void __cdecl sub_48A350(int a1, int a2, int a3, unsigned int a4, int a5, int a6) {
  // Check if we are below the maximum vertex count
  //FIXME: Not 100% sure
  if ( a4 <= dword_52E624 ) {

    // Prepare renderstates
    sub_48A450(a2);

    // Check if the planned texture is already set, if not, set it
    if ( a1 != dword_52E628 ) {
      //FIXME: This feels like a bug, either in the game or my RE..
      if (!dword_52E644->SetTexture(0, a1)) {
        // Update the current texture
        dword_52E628 = a1;
      }
    }

    // Draw the data
    dword_52E644->DrawIndexedPrimitive(4, 452, a3, a4, a5, a6, 24);
  }
}
```