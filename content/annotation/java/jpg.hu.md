---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java JPG Annotation API Annotate in C#"
head_description: "Java API népszerű kommentártípusok létrehozásához és megjegyzésekhez a JPG, képek, rajzok és dokumentumfájl formátumokból."

############################# Header ############################
title: "Jegyezze fel a(z) JPG fájlt Java-ból"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Ingyenes próbaverzió letöltése"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "A GroupDocs.Annotation for Java API-ról"
    content: |
        A GroupDocs.Annotation for Java API egy olyan könyvtár, amely lehetővé teszi megjegyzések hozzáadását PDF, Word és egyéb dokumentumokhoz Mac, Windows vagy Ubuntu rendszeren. A [GroupDocs.Annotation for Java](/annotation/java) egy natív Java API a kommentárok kezelésére, átfogó támogatással a megjegyzések létrehozásához, hozzáadásához, szerkesztéséhez, törléséhez, kibontásához és exportálásához képekből és különféle egyéb dokumentumokból. A támogatott dokumentumformátumok teljes listája ezen a [oldalon](https://docs.groupdocs.com/annotation/java/supported-document-formats/) tekinthető meg.
        Ez a könyvtár lehetővé teszi, hogy ne csak a JPG dokumentummal dolgozzon, hanem sok más típusú dokumentummal is, például Word, Excel, PowerPoint, Outlook e-mailekkel, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad és még sok mással.
        A GroupDocs.Annotation for Java API lehetővé teszi új jegyzetek létrehozását és hozzáadását, megjegyzések szerkesztését, megjegyzések kibontását, megjegyzések kibontását és eltávolítását a dokumentumokból. A könyvtár 13 különböző megjegyzéstípust támogat, beleértve a szöveget, vonalláncot, területet, aláhúzást, pontot, vízjelet, nyilat, ellipszist, szövegcserét, távolságot, szövegmezőt, erőforrás-szerkesztést PDF-ben, HTML-ben, Microsoft Word dokumentumokban, táblázatokban, diagramokban, prezentációkban, rajzok, képek és sok más fájlformátum.
        A példa (lásd alább) bemutatja a {{FÁJLFORMÁTUM}} dokumentummal való munkát, ebben a példában láthatja a GroupDocs használatának fő lépéseit. Annotáció: Állítson be egy licencet, nyissa meg a dokumentumot, amellyel dolgozni szeretne, és hozzon létre egy annotáció, adatobjektumok hozzáadása az annotációs tulajdonságok igényeinek megfelelő beállításához, és az eredmény mentése a kívánt helyre. A támogatott funkciókat a github [oldalon] (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) vagy a termékünk [dokumentációjában] (https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Lépések a megjegyzések hozzáadásához a JPG fájlhoz Java nyelven"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Néhány egyszerű lépés végrehajtásával megkönnyíti a Java fejlesztők számára, hogy különféle megjegyzéstípusokat adjanak hozzá a JPG fájlokhoz bármely Java-alapú alkalmazáson belül.
        *   Hozzon létre Válasz objektumokat megjegyzéssel és dátummal.
        *   Hozzon létre AreaAnnotation objektumot, állítsa be a terület beállításait és adjon hozzá válaszokat.
        *   Hozzon létre Annotator objektumot, és adjon hozzá terület megjegyzést.
        *   Mentse a kimeneti fájlt.
    title_right: "rendszerkövetelmények"
    content_right: |
        A GroupDocs.Annotation for Java API-kat minden nagyobb platformon és operációs rendszeren támogatja. Mielőtt végrehajtaná az alábbi kódot, győződjön meg arról, hogy a következő előfeltételek telepítve vannak a rendszeren.
        *   Operációs rendszerek: Microsoft Windows, Linux, MacOS
        *   Fejlesztési környezet: NetBeans, Intellij IDEA, Eclipse stb
        *   Java futási környezet: Java 7 (1.7) és újabb
        *   Szerezze be a GroupDocs.Annotation for Java legújabb verzióját a [GroupDocs Artifact Repository] webhelyről (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Annotáció előnézete és kódminta
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```java
        // Create an instance of Reply class and add comments
        Reply firstReply = new Reply();
        firstReply.setComment("First comment");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Second comment");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // Create an instance of AreaAnnotation class and set options
        AreaAnnotation area = new AreaAnnotation();
        area.setBackgroundColor(65535);
        area.setBox(new Rectangle(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("This is area annotation");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte) 3);
        area.setReplies(replies);
        
        // Create an instance of Annotator class
        Annotator annotator = new Annotator("input.bmp");
        
        // Add annotation
        annotator.add(area);
        
        // Save to file
        annotator.save("output.bmp");
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "A megjegyzések eltávolításának lépései a JPG fájlból Java nyelven"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Néhány egyszerű lépés végrehajtásával megkönnyíti a Java fejlesztők számára a megjegyzések részleteinek eltávolítását a JPG fájlokból bármely Java-alapú alkalmazásban.
        *   Hozzon létre Válasz objektumokat megjegyzéssel és dátummal.
        *   Példányosítsa a SaveOptions objektumot, és állítsa be az AnnotationTypes = AnnotationType.None beállítást.
        *   Hívja a mentési metódust az eredményül kapott dokumentumúttal vagy adatfolyammal és SaveOptions objektummal.

############################# Preview ############################
preview_Remove:
    enable: true
    code: |
        ```java
        // Create an instance of Annotator class 
        Annotator annotator = new Annotator("C://input.bmp");

        // Remove annotation by set type None 
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // Save annotation to output file
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "A JPG megjegyzéseinek szerkesztésének lépései Java nyelven"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Néhány egyszerű lépés végrehajtásával megkönnyíti a Java fejlesztők számára, hogy frissítsék a JPG fájlokból származó különféle megjegyzéstulajdonságokat bármely Java-alapú alkalmazáson belül.
        *   Példányosítása Annotator objektum bemeneti dokumentumútvonallal vagy adatfolyammal példányosított LoadOptions segítségével az ImportAnnotations = true értékkel.
        *   Hozzon létre valamilyen AnnotationBase implementációt, és állítsa be a létező annotáció azonosítóját (ha nem található annotáció ezzel az azonosítóval, akkor semmi sem módosul) vagy a megjegyzések elérési útlistáját (az összes létező annotációt eltávolítjuk).
        *   Az Annotator objektum frissítési metódusának hívása átadott megjegyzésekkel.
        *   Hívja a mentési metódust az eredményül kapott dokumentumúttal vagy adatfolyammal és SaveOptions objektummal.

############################# Preview ############################
preview_Edit:
    enable: true
    code: |
        ```java
        String outputPath = "UpdateAnnotation.bmp";

        // Create an instance of Annotator class
        Annotator annotator = new Annotator("input.bmp");
        
        // Create an instance of Reply class for first example and add comments
        Reply reply1 = new Reply();
        reply1.setComment("Original first comment");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Original second comment");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // Create an instance of AreaAnnotation class and set options
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("This is original annotation");
        original.setReplies(replies);
        
        // Add original annotation
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        
        // Open annotated document
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // Create an instance of Reply class for update first example
        Reply reply3 = new Reply();
        reply3.setComment("Updated first comment");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Updated second comment");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);

        // Suggest we want change some properties of existed annotation
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("This is updated annotation");
        updated.setReplies(replies1);
        
        // Update and save annotation
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Lépések a megjegyzések kibontásához a JPG fájlból Java nyelven"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) néhány egyszerű lépés végrehajtásával megkönnyíti a Java fejlesztők számára, hogy megjegyzéseket fűzzenek a dokumentumokhoz és kivonják a megjegyzésadatokat a JPG fájlokból bármely Java-alapú alkalmazáson belül.
        *   Hozzon létre Válasz objektumokat megjegyzéssel és dátummal.
        *   Példányosítsa a LoadOptions objektumot, és hívja meg a SetImportAnnotations-t igaz argumentummal.
        *   Definiáljon változót List típussal.
        *   Hívja meg a get metódust, és adja vissza az eredményt a fenti változóhoz.

############################# Preview ############################
preview_Extract:
    enable: true
    code: |
        ```java
        // For using this example input file ("annotated.bmp") must be with annotations
        LoadOptions loadOptions = new LoadOptions();
        
        // Create an instance of Annotator class and get annotations
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Élő bemutatók dokumentumok és képek megjegyzéseinek hozzáadásához, eltávolításához, szerkesztéséhez és kivonásához"
    content: |
        A [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) webhely meglátogatásával azonnal adhat hozzá, távolíthat el, szerkesszen és bontsa ki a megjegyzéseket a JPG fájlba. Az élő demónak a következő előnyei vannak

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-jpg"
          title: "A JPG fájlformátumról"
          content: |
            A JPG egy olyan képformátum, amelyet veszteséges tömörítés módszerével mentenek el. A kimeneti kép a tömörítés eredményeként kompromisszumot jelent a tárhely mérete és a képminőség között. A felhasználók beállíthatják a tömörítési szintet a kívánt minőségi szint eléréséhez, ugyanakkor csökkenthetik a tárhely méretét. A képminőséget elhanyagolható mértékben befolyásolja, ha 10:1-es tömörítést alkalmaznak a képen. Minél nagyobb a tömörítési érték, annál nagyobb a képminőség romlása.

          link: "https://docs.fileformat.com/image/jpg/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Más népszerű dokumentumformátumok használata"
    content: |
        Frissítse a megjegyzések tulajdonságait néhány népszerű fájlformátumból az alábbiak szerint.
    format:
        # format loop
        - name: "Annotate PDF document"
          link: "https://products.groupdocs.com/annotation/java/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Annotate DOC document"
          link: "https://products.groupdocs.com/annotation/java/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Annotate DOCM document"
          link: "https://products.groupdocs.com/annotation/java/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Annotate DOCX document"
          link: "https://products.groupdocs.com/annotation/java/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Annotate DOT document"
          link: "https://products.groupdocs.com/annotation/java/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Annotate DOTX document"
          link: "https://products.groupdocs.com/annotation/java/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Annotate RTF document"
          link: "https://products.groupdocs.com/annotation/java/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Annotate ODT document"
          link: "https://products.groupdocs.com/annotation/java/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Annotate XLS document"
          link: "https://products.groupdocs.com/annotation/java/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Annotate XLSX document"
          link: "https://products.groupdocs.com/annotation/java/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Annotate XLSM document"
          link: "https://products.groupdocs.com/annotation/java/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Annotate XLSB document"
          link: "https://products.groupdocs.com/annotation/java/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Annotate ODS document"
          link: "https://products.groupdocs.com/annotation/java/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Annotate PPT document"
          link: "https://products.groupdocs.com/annotation/java/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Annotate PPTX document"
          link: "https://products.groupdocs.com/annotation/java/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Annotate PPSX document"
          link: "https://products.groupdocs.com/annotation/java/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Annotate POTM document"
          link: "https://products.groupdocs.com/annotation/java/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Annotate PPTM document"
          link: "https://products.groupdocs.com/annotation/java/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Annotate PPS document"
          link: "https://products.groupdocs.com/annotation/java/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Annotate ODP document"
          link: "https://products.groupdocs.com/annotation/java/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Annotate HTML document"
          link: "https://products.groupdocs.com/annotation/java/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Annotate TIFF document"
          link: "https://products.groupdocs.com/annotation/java/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Annotate JPEG document"
          link: "https://products.groupdocs.com/annotation/java/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Annotate PNG document"
          link: "https://products.groupdocs.com/annotation/java/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Annotate EML document"
          link: "https://products.groupdocs.com/annotation/java/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Annotate MSG document"
          link: "https://products.groupdocs.com/annotation/java/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Annotate VSD document"
          link: "https://products.groupdocs.com/annotation/java/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Annotate VSDX document"
          link: "https://products.groupdocs.com/annotation/java/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Annotate VSS document"
          link: "https://products.groupdocs.com/annotation/java/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Annotate VST document"
          link: "https://products.groupdocs.com/annotation/java/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Annotate DWG document"
          link: "https://products.groupdocs.com/annotation/java/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Annotate DXF document"
          link: "https://products.groupdocs.com/annotation/java/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Annotate DCM document"
          link: "https://products.groupdocs.com/annotation/java/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Annotate WMF document"
          link: "https://products.groupdocs.com/annotation/java/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Annotate EMF document"
          link: "https://products.groupdocs.com/annotation/java/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---