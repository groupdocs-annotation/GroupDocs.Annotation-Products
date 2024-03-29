---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net HTML Annotation API Annotate in C#"
head_description: "Net API népszerű kommentártípusok létrehozásához és megjegyzések készítéséhez a HTML fájlokból, képekből, rajzokból és dokumentumfájl-formátumokból."

############################# Header ############################
title: "Jegyezze fel a(z) HTML fájlt a Netről"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Ingyenes próbaverzió letöltése"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "A GroupDocs.Annotation for Net API-ról"
    content: |
        A GroupDocs.Annotation for Net API egy olyan könyvtár, amely lehetővé teszi megjegyzések hozzáadását PDF, Word és egyéb dokumentumokhoz Mac, Windows vagy Ubuntu rendszeren. A [GroupDocs.Annotation for Net](/annotation/net) egy natív Net API a kommentárok kezelésére, átfogó támogatással a megjegyzések létrehozásához, hozzáadásához, szerkesztéséhez, törléséhez, kibontásához és exportálásához képekből és különféle egyéb dokumentumokból. A támogatott dokumentumformátumok teljes listája ezen a [oldalon](https://docs.groupdocs.com/annotation/net/supported-document-formats/) tekinthető meg.
        Ez a könyvtár lehetővé teszi, hogy ne csak a HTML dokumentummal dolgozzon, hanem sok más típusú dokumentummal is, például Word, Excel, PowerPoint, Outlook e-mailekkel, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad és még sok mással.
        A GroupDocs.Annotation for Net API lehetővé teszi új jegyzetek létrehozását és hozzáadását, megjegyzések szerkesztését, megjegyzések és megjegyzések kinyerését és eltávolítását a dokumentumokból. A könyvtár 13 különböző megjegyzéstípust támogat, beleértve a szöveget, vonalláncot, területet, aláhúzást, pontot, vízjelet, nyilat, ellipszist, szövegcserét, távolságot, szövegmezőt, erőforrás-szerkesztést PDF-ben, HTML-ben, Microsoft Word dokumentumokban, táblázatokban, diagramokban, prezentációkban, rajzok, képek és sok más fájlformátum.
        A példa (lásd alább) bemutatja a {{FÁJLFORMÁTUM}} dokumentummal való munkát, ebben a példában láthatja a GroupDocs használatának fő lépéseit. Annotáció: Állítson be egy licencet, nyissa meg a dokumentumot, amellyel dolgozni szeretne, és hozzon létre egy annotáció, adatobjektumok hozzáadása az annotációs tulajdonságok igényeinek megfelelő beállításához, és az eredmény mentése a kívánt helyre. A támogatott funkciókat a github [oldalon](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) vagy a termékünk [dokumentációjában](https://docs.groupdocs.com/annotation/net/getting-started/) tekintheti meg részletesebben is.

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Lépések a megjegyzések hozzáadásához a Net HTML fájlhoz"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Néhány egyszerű lépés végrehajtásával megkönnyíti a Net fejlesztői számára, hogy különféle megjegyzéstípusokat adjanak hozzá a HTML fájlokhoz bármely Net-alapú alkalmazáson belül.
        *   Hozzon létre Válasz objektumokat megjegyzéssel és dátummal.
        *   Hozzon létre AreaAnnotation objektumot, állítsa be a terület beállításait és adjon hozzá válaszokat.
        *   Hozzon létre Annotator objektumot, és adjon hozzá terület megjegyzést.
        *   Mentse a kimeneti fájlt.
    title_right: "rendszerkövetelmények"
    content_right: |
        A GroupDocs.Annotation for Net API-kat minden nagyobb platform és operációs rendszer támogatja. Mielőtt végrehajtaná az alábbi kódot, győződjön meg arról, hogy a következő előfeltételek telepítve vannak a rendszeren.
        *   Operációs rendszerek: Microsoft Windows, Linux, MacOS
        *   Fejlesztési környezetek: Visual Studio, Xamarin, MonoDevelop
        *   Keretrendszerek: .NET Framework, .NET Standard, .NET Core, Mono
        *   Töltse le a GroupDocs.Annotation for .NET legújabb verzióját a [NuGet] webhelyről (https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Annotáció előnézete és kódminta
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ```cs
        //Add text field annotation to the document from local disk
        using (Annotator annotator = new Annotator("input.bmp"))
        {
            TextFieldAnnotation textField = new TextFieldAnnotation
            {
                BackgroundColor = 65535,
                Box = new Rectangle(100, 100, 100, 100),
                CreatedOn = DateTime.Now,
                Text = "Some text",
                FontColor = 65535,
                FontSize = 12,
                Message = "This is text field annotation",
                Opacity = 0.7,
                PageNumber = 0,
                PenStyle = PenStyle.Dot,
                PenWidth = 3,
                FontFamily = "Arial",
                TextHorizontalAlignment = HorizontalAlignment.Center,
                Replies = new List
                {
                    new Reply
                    {
                        Comment = "First comment",
                        RepliedOn = DateTime.Now
                    },
                    new Reply
                    {
                        Comment = "Second comment",
                        RepliedOn = DateTime.Now
                    }
                }
            };
            annotator.Add(textField);
            annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "A megjegyzések eltávolításának lépései a Net HTML fájlból"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Néhány egyszerű lépés végrehajtásával megkönnyíti a Net fejlesztői számára a megjegyzések részleteinek eltávolítását a HTML fájlokból bármely Net-alapú alkalmazásban.
        *   Hozzon létre Válasz objektumokat megjegyzéssel és dátummal.
        *   Példányosítsa a SaveOptions objektumot, és állítsa be az AnnotationTypes = AnnotationType.None beállítást.
        *   Hívja a mentési metódust az eredményül kapott dokumentumúttal vagy adatfolyammal és SaveOptions objektummal.

############################# Preview ############################
preview_Remove:
    enable: true
    code: |
        ```cs
        // 1- How to remove annotation from document using annotation index
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            annotator.Remove(0);
            annotator.Save("removed.bmp");
        }
        
        // 2- How to remove annotation from document using annotation object
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp[0]);
            annotator.Save("removed.bmp");
        }
        
        // 3- How to remove some annotations from document using list of ID’s
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var idList = new List{1, 2, 3};
            annotator.Remove(idList);
            annotator.Save("removed.bmp");
        }
        
        // 4- How to remove some annotations from document using list of annotations
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp);
            annotator.Save("removed.bmp");
        }
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "A HTML megjegyzéseinek szerkesztésének lépései a Netben"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) néhány egyszerű lépés végrehajtásával megkönnyíti a Net fejlesztői számára a különféle megjegyzéstulajdonságok frissítését a HTML fájlokból bármely Net-alapú alkalmazáson belül.
        *   Példányosítása Annotator objektum bemeneti dokumentumútvonallal vagy adatfolyammal példányosított LoadOptions segítségével az ImportAnnotations = true értékkel.
        *   Hozzon létre valamilyen AnnotationBase implementációt, és állítsa be a létező annotáció azonosítóját (ha nem található annotáció ezzel az azonosítóval, akkor semmi sem módosul) vagy a megjegyzések elérési útlistáját (az összes létező annotációt eltávolítjuk).
        *   Az Annotator objektum frissítési metódusának hívása átadott megjegyzésekkel.
        *   Hívja a mentési metódust az eredményül kapott dokumentumúttal vagy adatfolyammal és SaveOptions objektummal.

############################# Preview ############################
preview_Edit:
    enable: true
    code: |
        ```cs
        // open annotated document
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            //assuming we are going to change some properties of existing annotation
                AreaAnnotation updated = new AreaAnnotation
                    {
                            // It's important to set existed annotation Id
                            Id = 1,
                            BackgroundColor = 255,
                            Box = new Rectangle(0, 0, 50, 200),
                            CreatedOn = DateTime.Now,
                            Message = "This is updated annotation",
                            Replies = new List
                            {
                                new Reply
                                {
                                    Comment = "Updated first comment",
                                    RepliedOn = DateTime.Now
                                },
                                new Reply
                                {
                                    Comment = "Updated second comment",
                                    RepliedOn = DateTime.Now
                                }
                            }
                        };
                // update annotation
                annotator.Update(updated);
                annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "A megjegyzések kinyerésének lépései a HTML fájlból a Netben"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) néhány egyszerű lépés végrehajtásával megkönnyíti a Net fejlesztői számára, hogy megjegyzéseket fűzzenek a dokumentumokhoz és kivonják a megjegyzésadatokat a HTML fájlokból bármely Net-alapú alkalmazáson belül.
        *   Hozzon létre Válasz objektumokat megjegyzéssel és dátummal.
        *   Példányosítsa a LoadOptions objektumot, és hívja meg a SetImportAnnotations-t igaz argumentummal.
        *   Definiáljon változót List típussal.
        *   Hívja meg a get metódust, és adja vissza az eredményt a fenti változóhoz.

############################# Preview ############################
preview_Extract:
    enable: true
    code: |
        ```cs
        // for using this example input file ("annotated.bmp") must be with annotations
        using (Annotator annotator = new Annotator("annotated.bmp"))
        {
            List annotations = annotator.Get();
            XmlSerializer formatter = new XmlSerializer(typeof(List));
            using (FileStream fs = new FileStream("annotations.xml", FileMode.Create))
            {
                fs.SetLength(0);
                formatter.Serialize(fs, annotations);
            }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Élő bemutatók dokumentumok és képek megjegyzéseinek hozzáadásához, eltávolításához, szerkesztéséhez és kivonásához"
    content: |
        A [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) webhely meglátogatásával azonnal adhat hozzá, távolíthat el, szerkesszen és bontsa ki a megjegyzéseket a HTML fájlba. Az élő demónak a következő előnyei vannak

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-html"
          title: "A HTML fájlformátumról"
          content: |
            A HTML (Hyper Text Markup Language) a böngészőben való megjelenítésre létrehozott weboldalak kiterjesztése. A web nyelveként ismert HTML a weboldalak részeként megjelenítendő új információs követelményekkel fejlődött. A legújabb változat HTML 5 néven ismert, amely nagy rugalmasságot biztosít a nyelvvel való munkavégzéshez. A HTML oldalak vagy a szerverről érkeznek, ahol ezeket tárolják, vagy a helyi rendszerről is betölthetők. Minden HTML-oldal HTML-elemekből áll, például űrlapokból, szövegekből, képekből, animációkból, hivatkozásokból stb. Ezeket az elemeket olyan címkék képviselik, mint például az img, a, p és még sok más, ahol minden címkének van eleje és vége. Szkriptnyelveken, például JavaScripten és stíluslapokon (CSS) írt alkalmazásokat is beágyazhat az általános elrendezés megjelenítéséhez.

          link: "https://docs.fileformat.com/image/html/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Más népszerű dokumentumformátumok használata"
    content: |
        Frissítse a megjegyzések tulajdonságait néhány népszerű fájlformátumból az alábbiak szerint.
    format:
        # format loop
        - name: "Annotate PDF document"
          link: "https://products.groupdocs.com/annotation/net/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Annotate DOC document"
          link: "https://products.groupdocs.com/annotation/net/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Annotate DOCM document"
          link: "https://products.groupdocs.com/annotation/net/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Annotate DOCX document"
          link: "https://products.groupdocs.com/annotation/net/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Annotate DOT document"
          link: "https://products.groupdocs.com/annotation/net/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Annotate DOTX document"
          link: "https://products.groupdocs.com/annotation/net/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Annotate RTF document"
          link: "https://products.groupdocs.com/annotation/net/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Annotate ODT document"
          link: "https://products.groupdocs.com/annotation/net/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Annotate XLS document"
          link: "https://products.groupdocs.com/annotation/net/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Annotate XLSX document"
          link: "https://products.groupdocs.com/annotation/net/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Annotate XLSM document"
          link: "https://products.groupdocs.com/annotation/net/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Annotate XLSB document"
          link: "https://products.groupdocs.com/annotation/net/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Annotate ODS document"
          link: "https://products.groupdocs.com/annotation/net/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Annotate PPT document"
          link: "https://products.groupdocs.com/annotation/net/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Annotate PPTX document"
          link: "https://products.groupdocs.com/annotation/net/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Annotate PPSX document"
          link: "https://products.groupdocs.com/annotation/net/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Annotate POTM document"
          link: "https://products.groupdocs.com/annotation/net/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Annotate PPTM document"
          link: "https://products.groupdocs.com/annotation/net/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Annotate PPS document"
          link: "https://products.groupdocs.com/annotation/net/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Annotate ODP document"
          link: "https://products.groupdocs.com/annotation/net/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Annotate HTML document"
          link: "https://products.groupdocs.com/annotation/net/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Annotate TIFF document"
          link: "https://products.groupdocs.com/annotation/net/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Annotate JPEG document"
          link: "https://products.groupdocs.com/annotation/net/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Annotate PNG document"
          link: "https://products.groupdocs.com/annotation/net/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Annotate EML document"
          link: "https://products.groupdocs.com/annotation/net/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Annotate MSG document"
          link: "https://products.groupdocs.com/annotation/net/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Annotate VSD document"
          link: "https://products.groupdocs.com/annotation/net/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Annotate VSDX document"
          link: "https://products.groupdocs.com/annotation/net/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Annotate VSS document"
          link: "https://products.groupdocs.com/annotation/net/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Annotate VST document"
          link: "https://products.groupdocs.com/annotation/net/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Annotate DWG document"
          link: "https://products.groupdocs.com/annotation/net/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Annotate DXF document"
          link: "https://products.groupdocs.com/annotation/net/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Annotate DCM document"
          link: "https://products.groupdocs.com/annotation/net/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Annotate WMF document"
          link: "https://products.groupdocs.com/annotation/net/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Annotate EMF document"
          link: "https://products.groupdocs.com/annotation/net/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---