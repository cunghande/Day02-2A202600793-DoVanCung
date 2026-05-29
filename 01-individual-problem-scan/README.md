# 01 - Individual Problem Scan

## Bang Scan Problems

| # | Lang kinh | Problem quan sat duoc | Ai dang dau? | Dau hieu that |
|---:|---|---|---|---|
| 1 | Ton thoi gian | Tong hop tai lieu on thi tu nhieu nguon | Sinh vien | Mat 2-3 gio truoc moi ky thi de gom slide, PDF, de cuong va ghi chu |
| 2 | AI co the tot hon | Doc paper AI de lay y chinh | Sinh vien AI | Mat 20-30 phut cho moi paper, de bo sot methodology hoac limitation |
| 3 | Lap lai | Tim lai thong tin trong Discord/Zalo lop | Sinh vien | Mat 10-15 phut moi lan tim deadline, link nop bai hoac cau tra loi cu |
| 4 | Pain tu nguoi khac | Thanh vien nhom khong nam duoc tien do do an | Nhom do an | Thanh vien hoi lai nhieu lan ve viec ai dang lam gi, viec nao da xong |
| 5 | Ton thoi gian | Viet bao cao mon hoc | Sinh vien | Phai sua nhieu lan ve format, cau truc va noi dung |
| 6 | Lap lai | Theo doi deadline nhieu mon hoc | Sinh vien | Deadline nam rai rac o LMS, Zalo, email; de quen han hoac nop sat han |
| 7 | AI co the tot hon | Tim de tai nghien cuu phu hop | Sinh vien AI | Mat nhieu thoi gian tim paper, so sanh do kho va muc do phu hop |
| 8 | Pain tu nguoi khac | Nguoi moi kho hieu he thong do an | Thanh vien moi | Phai giai thich lai kien truc, cach chay project va quy uoc nhom |

## Top 3 Problems

| Rank | Problem | Vi sao chon | Dieu con chua chac |
|---:|---|---|---|
| 1 | Tong hop tai lieu on thi | Pain that, xay ra truoc moi ky thi, ton nhieu thoi gian va co the do bang thoi gian tao outline on tap | Chat luong tom tat cua AI va kha nang bo sot kien thuc quan trong |
| 2 | Tim lai thong tin Discord/Zalo | Nhieu sinh vien gap, workflow ro va impact do duoc bang thoi gian tim kiem | Kho lay du lieu tu Zalo/Discord va can xu ly quyen rieng tu |
| 3 | Theo doi deadline mon hoc | De do hieu qua, lien quan truc tiep den viec nop bai dung han | Co the chi can Rule/Calendar, khong nhat thiet can AI |

---

## Problem Card #1 - Tong hop tai lieu on thi

### Problem 1 cau

Sinh vien mat nhieu thoi gian tong hop tai lieu on thi tu nhieu nguon khac nhau truoc ky thi.

### Actor

Sinh vien dai hoc.

### Thoi diem / boi canh

Truoc ky thi giua ky hoac cuoi ky, khi sinh vien can gom slide bai giang, PDF tham khao, de cuong mon hoc va ghi chu cu de tao tai lieu on tap.

### Current Workflow

| Buoc | Actor | Input | Output | Thoi gian |
|---:|---|---|---|---|
| 1 | Sinh vien | Slide bai giang | Danh sach slide can doc | 10 phut |
| 2 | Sinh vien | PDF tham khao | Tai lieu tham khao lien quan | 15 phut |
| 3 | Sinh vien | De cuong mon hoc | Cac chu de can on | 5 phut |
| 4 | Sinh vien | Tat ca tai lieu | Ghi chu tam | 90 phut |
| 5 | Sinh vien | Ghi chu tam | Tai lieu on tap ban dau | 30 phut |

### Current Workflow Diagram

```text
[Slide]
   \
    \
     > [Doc tai lieu] ---> [Ghi chu tam] ---> [Tai lieu on tap]
    /
   /
[PDF]

[De cuong] ----------------^
```

### Bottleneck

Doc, loc y chinh va tong hop tai lieu mat khoang 120 phut.

### Impact

Sinh vien ton nhieu thoi gian truoc ky thi, de bo sot kien thuc quan trong hoac tao tai lieu on tap thieu cau truc.

### Success Metric

Giam thoi gian tao ban nhap outline on tap tu khoang 3 gio xuong duoi 30 phut. Sinh vien van phai review noi dung truoc khi dung de hoc.

### Non-AI Alternative

Dung template ghi chu va checklist on tap theo tung mon.

### AI Hypothesis

AI ho tro tom tat slide/PDF/de cuong, gom y trung nhau, tao outline on tap va danh dau phan can sinh vien kiem tra lai.

### Quick Gut

Workflow.

### Future Workflow

```text
[Slide + PDF + De cuong]
            |
            v
      [AI tom tat]
            |
            v
    [AI tao outline]
            |
            v
   [Sinh vien review]
            |
            v
 [Tai lieu on tap da kiem tra]
```

### Human Boundary

Sinh vien phai kiem tra lai noi dung, doi chieu voi de cuong va slide goc truoc khi hoc hoac chia se cho nguoi khac.

---

## Problem Card #2 - Tim lai thong tin Discord/Zalo lop

### Problem 1 cau

Sinh vien mat nhieu thoi gian tim lai thong tin cu trong Discord hoac Zalo lop.

### Actor

Sinh vien.

### Thoi diem / boi canh

Khi can tim lai deadline, link nop bai, file tai lieu, quyet dinh cua nhom/lop hoac cau tra loi cu trong cac kenh chat.

### Current Workflow

```text
[Mo Discord/Zalo]
        |
        v
  [Search tu khoa]
        |
        v
[Doc nhieu tin nhan]
        |
        v
[Tim duoc thong tin]
```

### Bottleneck

Phai doc lai nhieu tin nhan, thu nhieu tu khoa khac nhau va de bo sot thong tin neu khong nho dung cach nguoi khac da viet.

### Impact

Moi lan tim mat 10-15 phut; neu tim sai hoac khong thay co the nop bai muon, hoi lai ban cung lop hoac lam theo thong tin cu.

### Success Metric

Giam thoi gian tim thong tin tu 10-15 phut xuong duoi 1 phut, ket qua tra ve phai kem nguon/tin nhan goc de nguoi dung xac nhan.

### Non-AI Alternative

Pin cac thong tin quan trong, tao FAQ hoac document tong hop link/deadline.

### AI Hypothesis

Semantic search giup sinh vien hoi bang ngon ngu tu nhien va tra ve thong tin lien quan kem link/tin nhan goc.

### Quick Gut

Workflow.

### Future Workflow

```text
[Nhap cau hoi]
       |
       v
[AI semantic search]
       |
       v
[Tra ket qua + nguon]
       |
       v
[Nguoi dung xac nhan]
```

### Human Boundary

Nguoi dung can kiem tra nguon goc vi AI co the lay nham tin nhan cu, sai ngu canh hoac bo sot thong bao moi hon.

---

## Problem Card #3 - Theo doi deadline mon hoc

### Problem 1 cau

Sinh vien gap kho khan khi theo doi deadline cua nhieu mon hoc cung luc.

### Actor

Sinh vien.

### Thoi diem / boi canh

Trong hoc ky, khi deadline bai tap, quiz, project va bao cao duoc thong bao o nhieu noi nhu LMS, email, Zalo lop hoac loi nhac cua giang vien.

### Current Workflow

```text
[LMS]
   |
   v
[Zalo lop]
   |
   v
[Email]
   |
   v
[Ghi chu thu cong]
   |
   v
[Theo doi deadline]
```

### Bottleneck

Thong tin deadline nam o nhieu noi, sinh vien phai tu kiem tra va ghi lai thu cong.

### Impact

Sinh vien de quen deadline, nop sat han hoac bo sot yeu cau nho trong thong bao.

### Success Metric

100% deadline duoc ghi vao calendar trong vong 24 gio sau khi duoc thong bao. Nhac truoc han 3 ngay va 1 ngay. So lan quen deadline trong mot hoc ky giam tu 2-3 lan xuong 0 lan.

### Non-AI Alternative

Google Calendar, checklist theo mon va reminder lap lai.

### AI Hypothesis

AI co the doc thong bao tu nhieu nguon, nhan dien deadline, trich xuat ten mon, yeu cau nop bai va de xuat lich nhac.

### Quick Gut

Rule.

### Future Workflow

```text
[LMS + Email + Zalo]
          |
          v
[Tong hop deadline]
          |
          v
[Calendar tap trung]
          |
          v
[Nhac truoc han]
          |
          v
[Hoan thanh bai tap]
```

### Human Boundary

Sinh vien can xac nhan deadline truoc khi them vao calendar, dac biet khi thong bao bi sua hoac co nhieu moc nop bai khac nhau.

---

## Card muon pitch nhat

### Card toi muon pitch nhat

Problem Card #1 - Tong hop tai lieu on thi tu nhieu nguon.

### Vi sao

Day la pain that cua sinh vien truoc moi ky thi, xay ra lap lai o nhieu mon, ton nhieu thoi gian va co the do duoc bang thoi gian chuan bi tai lieu on tap. Bai nay cung phu hop de so sanh giua template ghi chu, workflow ho tro va AI tom tat.

### Cau hoi toi muon nhom challenge

- AI tom tat co lam mat hoac hieu sai kien thuc quan trong khong?
- Lam sao kiem tra chat luong outline on tap?
- Bai nay nen dung AI o muc Workflow hay chi can template + checklist?
