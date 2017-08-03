# IQA
I = imread('people_in_paris2.jpg');
figure()
imshow(I)
imfinfo('people_in_paris2.jpg')

Igray = rgb2gray(I);
imshow(Igray);
level=0.4;
Ithresh = imbinarize(Igray, level);
%imshowpair(I, Ithresh, 'montage');
imshow(Ithresh)
print -djpeg

%%
I = imread('ny_tsquare.jpg');
figure()
imshow(I)
imfinfo('ny_tsquare.jpg')

Igray = rgb2gray(I);
imshow(Igray);
%%
I = imread('bob_rose_original.jpg');
figure()
imshow(I)
imfinfo('bob_rose_original.jpg')
Igray = rgb2gray(I);
imshow(Igray);
%%
level=0.4;
Ithresh = imbinarize(Igray, level);
%imshowpair(I, Ithresh, 'montage');
subplot(221)
imshow(Ithresh)

level=0.5;
Ithresh = imbinarize(Igray, level);
subplot(222)
imshow(Ithresh)

level=0.6;
Ithresh = imbinarize(Igray, level);
subplot(223)
imshow(Ithresh)

level=0.7;
Ithresh = imbinarize(Igray, level);
subplot(224)
imshow(Ithresh)

%%
I = imread('monalisa.jpg');
figure()
imshow(I)
imfinfo('monalisa.jpg')
%%
Igray = rgb2gray(I);
imshow(Igray);
%%
I = imread('niagara.jpg');
figure()
imshow(I)
imfinfo('niagara.jpg')
Igray = rgb2gray(I);
imshow(Igray);
