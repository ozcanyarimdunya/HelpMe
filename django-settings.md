## settings.py

    BASE_DIR is where settings.py in.

    TEMPLATES = os.path.join(BASE_DIR,'templates')

    Everytime you create template create a base.html and MUST contain a block named content | 
    | you may have head_title block
    
    
    STATIC_URL = '/static/'
    
    if DEBUG:
      MEDIA_URL = '/media/'

      STATIC_ROOT = os.path.joins(BASE_DIR,'static','static_only')
      MEDIA_ROOT = os.path.joins(BASE_DIR,'static','media')

      STATICFILES_DIRS = [ os.path.join(BASE_DIR,'static','static') ]


## urls.py
-----------

    from django.conf import settings

    if settings.DEBUG:
        urlpatterns += static(settings.STATIC_URL,document_root=settings.STATIC_ROOT)
        urlpatterns += static(settings.MEDIA_URL,document_root=settings.MEDIA_ROOT)


