---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net VSS Annotation API Annotate C#-ում"
head_description: "Net API՝ VSS-ից հայտնի ծանոթագրությունների տեսակներ ստեղծելու և ծանոթագրելու համար, պատկերներ, գծագրեր և փաստաթղթերի ֆայլերի ձևաչափեր:"

############################# Header ############################
title: "Նշեք VSS-ը Net-ից"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Ներբեռնեք անվճար փորձաշրջան"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "GroupDocs.Annotation-ի մասին Net API-ի համար"
    content: |
        GroupDocs.Annotation-ը Net API-ի համար գրադարան է, որը թույլ է տալիս անոտացիաներ ավելացնել PDF, Word և այլ փաստաթղթեր Mac-ում, Windows-ում կամ Ubuntu-ում: [GroupDocs.Annotation for Net](/annotation/net) բնիկ Net API-ն է՝ ծանոթագրությունները կառավարելու համար՝ պատկերներից և տարբեր այլ փաստաթղթերից ծանոթագրություններ ստեղծելու, ավելացնելու, խմբագրելու, ջնջելու, հանելու և արտահանելու համապարփակ աջակցությամբ: Աջակցվող փաստաթղթերի ձևաչափերի ամբողջական ցանկը, որոնք կարող եք տեսնել այս [էջում](https://docs.groupdocs.com/annotation/net/supported-document-formats/):
        Այս գրադարանը թույլ է տալիս աշխատել ոչ միայն VSS փաստաթղթի, այլ նաև բազմաթիվ այլ տեսակի փաստաթղթերի հետ, ինչպիսիք են Word, Excel, PowerPoint, Outlook էլ. նամակներ, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad և շատ այլ փաստաթղթեր:
        GroupDocs.Annotation-ը Net API-ի համար թույլ է տալիս ստեղծել և ավելացնել նոր նշումներ, խմբագրել ծանոթագրությունները, հանել մեկնաբանություններ, ծանոթագրություններ և հեռացնել դրանք փաստաթղթերից: Գրադարանը աջակցում է անոտացիայի 13 տարբեր տեսակների, այդ թվում՝ տեքստ, պոլիգիծ, տարածք, ընդգծում, կետ, ջրանիշ, սլաք, էլիպս, տեքստի փոխարինում, հեռավորություն, տեքստային դաշտ, ռեսուրսների խմբագրում PDF, HTML, Microsoft Word փաստաթղթերում, աղյուսակներ, դիագրամներ, ներկայացումներ, գծագրեր, պատկերներ և շատ այլ ֆայլերի ձևաչափեր:
        Օրինակը (տես ստորև) ցույց է տալիս աշխատանքը VSS փաստաթղթի հետ, այս օրինակում կարող եք տեսնել GroupDocs-ի հետ աշխատելու հիմնական քայլերը: Ծանոթագրություն. Կարգավորեք լիցենզիա, բացեք փաստաթուղթ, որի հետ ցանկանում եք աշխատել, ստեղծելով անոտացիա՝ ավելացնելով տվյալների օբյեկտներ՝ ձեր պահանջներին համապատասխան անոտացիոն հատկություններ սահմանելու համար և արդյունքը պահելով անհրաժեշտ տեղում: Նաև կարող եք ավելի մանրամասն նայել մեր github-ի [էջի աջակցվող գործառույթներին](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) կամ մեր արտադրանքի [փաստաթղթերում](https://docs.groupdocs.com/annotation/net/getting-started/):

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "VSS-ին Net-ում ծանոթագրություններ ավելացնելու քայլեր"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) հեշտացնում է Net ծրագրավորողներին ավելացնել անոտացիայի տարբեր տեսակներ VSS ֆայլերում ցանցի վրա հիմնված ցանկացած հավելվածի մեջ՝ իրականացնելով մի քանի հեշտ քայլեր:
        *   Ստեղծեք Reply օբյեկտներ՝ մեկնաբանությամբ և ամսաթվով:
        *   Ստեղծեք AreaAnnotation օբյեկտ, սահմանեք տարածքի ընտրանքները և ավելացրեք պատասխաններ:
        *   Ստեղծեք Annotator օբյեկտ և ավելացրեք տարածքի անոտացիա:
        *   Պահպանեք ելքային ֆայլը:
    title_right: "Համակարգի պահանջները"
    content_right: |
        GroupDocs.Annotation-ը Net API-ների համար աջակցվում է բոլոր հիմնական հարթակներում և օպերացիոն համակարգերում: Նախքան ստորև նշված կոդը գործարկելը, համոզվեք, որ ձեր համակարգում տեղադրված են հետևյալ նախադրյալները.
        *   Օպերացիոն համակարգեր՝ Microsoft Windows, Linux, MacOS
        *   Զարգացման միջավայրեր՝ Visual Studio, Xamarin, MonoDevelop
        *   Frameworks՝ .NET Framework, .NET Standard, .NET Core, Mono
        *   Ներբեռնեք GroupDocs.Annotation-ի վերջին տարբերակը .NET-ի համար [NuGet]-ից (https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Անոտացիայի նախադիտում և կոդի նմուշ
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
    title_left: "Ծանոթագրությունները VSS-ից Net-ից հեռացնելու քայլեր"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) հեշտացնում է Net ծրագրավորողների համար անոտացիայի մանրամասները VSS ֆայլերից հեռացնելը ցանցի վրա հիմնված ցանկացած հավելվածում` իրականացնելով մի քանի հեշտ քայլեր:
        *   Ստեղծեք Reply օբյեկտներ՝ մեկնաբանությամբ և ամսաթվով:
        *   Տեղադրեք SaveOptions օբյեկտը և սահմանեք AnnotationTypes = AnnotationType.None:
        *   Զանգահարեք պահպանման մեթոդը՝ ստացված փաստաթղթի ճանապարհով կամ հոսքով և SaveOptions օբյեկտով:

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
    title_left: "VSS-ից Net-ում ծանոթագրությունները խմբագրելու քայլեր"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) հեշտացնում է Net ծրագրավորողների համար թարմացնել անոտացիայի տարբեր հատկություններ VSS ֆայլերից ցանցի վրա հիմնված ցանկացած հավելվածում` իրականացնելով մի քանի հեշտ քայլեր:
        *   Instantiate Annotator օբյեկտը մուտքագրված փաստաթղթի ուղով կամ հոսք՝ instantiated LoadOptions-ով ImportAnnotations-ով = true:
        *   Ստեղծեք AnnotationBase-ի ներդրում և սահմանեք գոյություն ունեցող անոտացիայի ID-ն (եթե այդ ID-ով ծանոթագրությունը չի գտնվել, ոչինչ չի փոխվի) կամ ծանոթագրությունների ուղու ցանկը (բոլոր գոյություն ունեցող ծանոթագրությունները կհեռացվեն):
        *   Annotator օբյեկտի զանգի թարմացման եղանակը՝ անցած ծանոթագրություններով:
        *   Զանգահարեք պահպանման մեթոդը՝ ստացված փաստաթղթի ճանապարհով կամ հոսքով և SaveOptions օբյեկտով:

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
    title_left: "Քայլեր՝ ծանոթագրություններ հանելու VSS-ից Net-ում"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) հեշտացնում է Net ծրագրավորողներին ծանոթագրել փաստաթղթերը և անոտացիոն տեղեկություններ հանել VSS ֆայլերից ցանցի վրա հիմնված ցանկացած հավելվածում՝ մի քանի հեշտ քայլեր իրականացնելով:
        *   Ստեղծեք Reply օբյեկտներ՝ մեկնաբանությամբ և ամսաթվով:
        *   Instantiate LoadOptions օբյեկտը և կանչեք SetImportAnnotations ճշմարիտ արգումենտով:
        *   Սահմանել փոփոխականը «List» տիպով:
        *   Զանգահարեք ստացման մեթոդը և վերադարձրեք արդյունքը վերը նշված փոփոխականին:

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
    title: "Կենդանի ցուցադրություններ՝ փաստաթղթերի և պատկերների վրա ավելացնելու, հեռացնելու, խմբագրելու, ծանոթագրություններ հանելու համար"
    content: |
        Ավելացրեք, հեռացրեք, խմբագրեք և հանեք ծանոթագրություններ VSS ֆայլում հենց հիմա՝ այցելելով [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) կայքը: Կենդանի ցուցադրությունն ունի հետևյալ առավելությունները

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-vss"
          title: "VSS Ֆայլի ձևաչափի մասին"
          content: |
            VSS-ը տրաֆարետային ֆայլեր են, որոնք ստեղծվել են Microsoft Visio 2007-ով և ավելի վաղ: Համեմատաբար նոր ֆայլի ձևաչափը .VSSX-ն է, որը ներկայացվել է Microsoft Visio 2013-ի հետ միասին: Տաբատային ֆայլերը ապահովում են գծագրման առարկաներ, որոնք կարող են ներառվել .VSD Visio գծագրում: Microsoft Visio-ն ինքնին հայտնի է գծագրության տարրեր ստեղծելով, ինչպիսիք են ձևերի հավաքածուն, միակցիչները, հոսքային գծապատկերները, ցանցի դասավորությունը, UML դիագրամները, ծրագրային ապահովման դիագրամները, տվյալների բազայի մոդելները, օբյեկտների քարտեզագրումը և նմանատիպ այլ տեղեկություններ: Այն նաև ունի Visio փաստաթղթերի փոխակերպման հարուստ հնարավորություններ այլ ֆայլերի ձևաչափերի, ինչպիսիք են PNG, BMP, PDF և այլն: Visio-ն հասանելի է ինչպես Windows-ի, այնպես էլ Mac OS-ի համար:

          link: "https://docs.fileformat.com/image/vss/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Աշխատեք փաստաթղթի այլ հանրաճանաչ ձևաչափերի հետ"
    content: |
        Թարմացրեք ծանոթագրության հատկությունները որոշ հայտնի ֆայլերի ձևաչափերից, ինչպես նշված է ստորև:
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