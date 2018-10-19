# mpdf_watermarks
mPDF 5.6, with minor changes to support:
 * multiline watermarks
 * watermark color
 * watermark location

Usage:
        // Init mPdf
        $mpdf = new mPDF();
        $mpdf->SetImportUse();
        $mpdf->SetSourceFile($sourceFile);
        
        // Multiline watermarks
        $mpdf->SetWatermarkText(['line1', 'line2', 'line3']);
        $mpdf->showWatermarkText = true;
        
        // Watermark color
        $mpdf->watermarkColor     = '#00FFFF';
        $mpdf->watermarkTextAlpha = 0.8;
        
        // Watermark location
        $mpdf->watermark_y_location = 20;
        $mpdf->watermark_x_location = 1;
